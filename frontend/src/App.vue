<template>
  <router-view />
</template>

<style lang="scss">
html,
body,
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.logoLogin {
  // Logo /login & /signup
  height: 10rem;
  margin-bottom: 2rem;
}

.btn {
  border: 1px solid rgb(233, 67, 38);
  background-color: white;
  border-radius: 0.3rem;
  padding: 0.2rem 1rem;
  color: rgb(233, 67, 38);
  font-weight: bold;
  &:hover {
    cursor: pointer;
  }
}

// Style des formulaires LoginForm.vue & SignupForm.vue
.form {
  background-color: rgb(255, 245, 245);
  border: 2px solid rgb(233, 67, 38);
  padding: 3rem 7rem;
  border-radius: 0.5rem;
  margin: 0 auto;
  text-align: left;
  &--input {
    margin-bottom: 1rem;
    width: 20rem;
    outline-color: rgb(233, 67, 38);
  }
  &--div {
    display: flex;
    justify-content: space-between;
    &__bg {
      // div qui prend tout le viewport et qui contient les formulaires
      height: 100vh;
      width: 100vw;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      img {
        margin: 2rem 0;
      }
    }
  }
  p {
    width: 20rem;
  }
}
.warning {
  color: red;
  margin-bottom: 0.7rem;
}

@media (max-width: 550px) {
  // Style des formulaires LoginForm.vue & SignupForm.vue
  .form {
    margin: 0.5rem;
    padding: 4rem;
    &--input {
      margin-bottom: 1rem;
      width: 100%;
      outline-color: rgb(233, 67, 38);
    }
    &--div {
      display: flex;
      justify-content: space-between;
      a {
        margin-right: 1rem;
      }
      &__bg {
        // div qui prend tout le viewport et qui contient les formulaires
        width: 100%;
        height: 100vh;
        display: flex;
        img {
          margin: 2rem 0;
        }
      }
    }
    p {
      width: 100%;
    }
  }
}
</style>
