<script setup>

</script>

<template>
  <div class="form-wrapper">
    <div class="form-wrapper__body">
      <form
        action=""
        method="post"
        class="form-wrapper__body-form form"
      >
        <img
          class="form-wrapper__body-image"
          src="@/assets/icons/logo.svg"
          alt=""
          width="72" height="72"
        >
        <div class="form__login">
          <h3 class="form__login-title h2">Login to your Account</h3>
          <p class="form__login-description">See what is going on with your business</p>
        </div>
        <label for="email" class="form__label">
          Email
        </label>
        <input
          class="form__input"
          type="email"
          name="email"
          placeholder="mail@abc.com"
          id="email"
        >
        <label for="password" class="form__label">
          Password
        </label>
        <input
          class="form__input"
          type="password"
          name="password"
          placeholder="password"
          id="password"
        >
        <div class="form__row">
          <label for="checkbox" class="form__label">
            <input
              class="form__label-checkbox"
              type="checkbox"
              name="checkbox"
              id="checkbox"
            >
            Remember me
          </label>
          <a href="" class="form__row-forget-password">Forgot Password?</a>
        </div>
        <button class="form__button" type="submit">
          Login
        </button>
      </form>
      <div class="form-wrapper__body-bottom form__bottom">
        <ul class="form__bottom-list">
          <li class="form__bottom-list__item">
            Not Registered Yet?
          </li>
          <li class="form__bottom-list__item">
            <a href="" class="form__bottom-list__item-link">Create an account</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.form-wrapper {
  justify-content: space-between;
  background-color: var(--color-light);
  max-width: rem(800);
  width: 100%;

  &__body {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
    padding: rem(80) rem(180) rem(50) rem(190);
  }
}

.form {
  display: flex;
  flex-direction: column;
  align-items: start;
  max-width: rem(430);

  &__login {
    padding: 0 rem(26);
    margin-top: rem(36);
  }

  &__label {
    margin-block: rem(24) rem(4);
  }

  &__input {
    line-height: 1.5;
    max-width: rem(420);
    width: 100%;
    padding: rem(13) rem(10);
    border:rem(1) solid var(--input-stroke);
    border-radius: rem(5);

    &::placeholder {
      color: var(--input-placeholder);
    }

    &:hover {
      border-color: var(--color-accent);
    }
  }

  &__row {
    display: flex;
    justify-content: space-between;
    max-width: rem(420);
    width: 100%;


    &-forget-password {
      margin-block: rem(24) rem(4);
    }
  }

  &__label {
    &-checkbox[type=checkbox]:checked {
      accent-color: var(--color-accent);
    }
  }

  &__button {
    align-self: center;
    background-color: var(--color-accent);
    font-size: rem(18);
    font-weight: 800;
    color: var(--color-light);
    max-width: rem(420);
    width: 100%;
    margin-top: rem(28);
    padding: rem(14) 0;
    border: none;
    border-radius: rem(6);

    @include hover {
      background-color: var(--color-grey);
    }
  }
}

.form__bottom {
  max-width: rem(420);

  &-list {
    display: flex;
    justify-content: center;
    column-gap: rem(10);
  }
}
</style>
