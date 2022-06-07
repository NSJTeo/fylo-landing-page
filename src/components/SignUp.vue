<template>
  <div className="sign-up__background">
    <div className="sign-up__container">
      <p className="sign-up__header">Get Early Access Today</p>
      <p className="sign-up__text">
        It only takes a minute to sign up and our free starter tier is extremely
        generous. If you have any questions, our support team would be happy to
        help you.
      </p>
      <form className="sign-up__form" @submit="handleSubmit">
        <input
          type="email"
          className="sign-up__input"
          placeholder="email@example.com"
          required
          v-model="email"
        />
        <button className="sign-up__button" type="submit">
          Get Started For Free
        </button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SignUp',
  data() {
    return {
      email: '',
    };
  },
  methods: {
    handleSubmit(e) {
      e.preventDefault();
      this.email = '';
    },
  },
};
</script>

<style lang="scss">
@use '../styles/variables.scss' as *;

.sign-up {
  &__background {
    padding: 0 20px;
    display: flex;
    justify-content: center;
    position: relative;
    top: 160px;
  }
  &__container {
    background: #1b2330;
    box-shadow: 5px 5px 8px rgba(0, 0, 0, 0.254274);
    border-radius: 9px;
    max-width: 863px;
    padding: 28px 40px 28px 37px;
  }
  &__header {
    margin-bottom: 1rem;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 24px;
    color: #ffffff;
    text-align: center;
  }
  &__text {
    margin-bottom: 2rem;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    color: #ffffff;
  }
  &__form {
    display: flex;
    flex-direction: column;
  }
  &__input {
    border: none;
    margin-bottom: 24px;
    padding: 19px 0 15px 29px;
    background: #ffffff;
    box-shadow: 1px 1px 3px rgba(7, 4, 59, 0.157043);
    border-radius: 24px;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 10px;
    line-height: 14px;
    color: #07043b;
    &::placeholder {
      font-family: 'Open Sans';
      font-style: normal;
      font-weight: 400;
      font-size: 10px;
      line-height: 14px;
      color: #c0c0c0;
    }
  }
  &__button {
    padding: 1rem 0;
    background: linear-gradient(132.02deg, #63e1d9 -31.85%, #34a0cd 100%);
    box-shadow: 2px 3px 6px rgba(0, 0, 0, 0.15925);
    border-radius: 24px;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 14px;
    line-height: 16px;
    color: #ffffff;
    border: none;
  }
}
</style>
