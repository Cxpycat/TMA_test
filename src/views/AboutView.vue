<template>
  <div class="profile_app">
    <div class="data_wrapper">
      <h3>Create profile</h3>

      <div class="name_wrapper">
        <input class="text-field__input" type="text" placeholder="Name">
        <div class="description_wrapper">
          <input class="text-field__input" type="text" id="about" placeholder="About you">
          <div class="text-secondary">Example: Designer from Dubai<br>Max. 140 characters</div>
        </div>
      </div>

      <div class="instagram_wrapper">
        <div class="description_wrapper">
          <div class="text-field__icon text-field__icon_instagram">
            <input class="text-field__input" type="text" id="instagram" placeholder="instagram.com/">
          </div>
          <label class="text-secondary" for="instagram">Instagram profile must be public</label>
        </div>
      </div>

      <div class="date_and_city_wrapper">
        <input class="text-field__input" type="date" value="2022-01-01" placeholder="Date of birth">
        <input class="text-field__input" type="text" placeholder="Your city">
      </div>

      <div class="gender_wrapper">
        <div class="form_radio_btn">
          <input id="radio-1" type="radio" name="radio" value="1" checked>
          <label for="radio-1">Male</label>
        </div>

        <div class="form_radio_btn">
          <input id="radio-2" type="radio" name="radio" value="0">
          <label for="radio-2">Female</label>
        </div>
      </div>
    </div>

    <button type="button" class="btn btn-black">Continue</button>
  </div>
</template>

<script>
export default {
  name: 'AboutView'
}
</script>

<style scoped>
.profile_app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-radius: 1rem;
  flex: 1;
  width: 100%;
}

.data_wrapper {
  flex: 1;
  width: 100%;
  height: 100%;
}

.name_wrapper,
.date_and_city_wrapper,
.instagram_wrapper {
  margin-top: 1rem;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.gender_wrapper {
  display: flex;
  flex-direction: row;
  gap: 1rem;
  margin-top: 1rem;
  align-items: center;
  justify-content: center;
}

.description_wrapper {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.text-field__icon_instagram::before {
  width: 1rem;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 448 512'%3E%3C!--!Font Awesome Free 6.6.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--%3E%3Cpath d='M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z'/%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: center;
}
</style>
