<template>
  <div className="hero__background">
    <div className="hero__container">
      <img
        className="hero__illustration"
        src="../assets/illustrations/illustration-intro.png"
        alt=""
      />
      <p className="hero__header">
        All your files in one secure location, accessible anywhere.
      </p>
      <p className="hero__text">
        Fylo stores all your most important files in one secure location. Access
        them wherever you need, share and collaborate with friends family, and
        co-workers.
      </p>
      <div className="hero__button-container">
        <button className="hero__button">Get Started</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero',
};
</script>

<style lang="scss">
@use '../styles/variables.scss' as *;
@use '../styles/mixins.scss' as *;

.hero {
  &__background {
    padding-top: 48px;
    background-image: url(../assets/backgrounds/bg-curvy-mobile.svg);
    background-color: $background-secondary;
    background-size: 100vw;
    background-repeat: no-repeat;
    background-position: 0 14.5rem;
    @include desktop {
      padding-top: 75px;
    }
  }
  &__container {
    margin-bottom: 131.22px;
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 1440px;
    margin: 0 auto;
  }
  &__illustration {
    height: 225px;
    margin-bottom: 33px;
    padding: 0 36px;
    @include desktop {
      height: 534px;
      margin-bottom: 36px;
    }
  }
  &__header {
    margin-bottom: 15px;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    line-height: 36px;
    text-align: center;
    color: #ffffff;
    padding: 0 28px;
    @include desktop {
      font-size: 40px;
      line-height: 60px;
      margin-bottom: 32px;
      max-width: 734px;
    }
  }
  &__text {
    margin-bottom: 32px;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    color: #ffffff;
    padding: 0 40px;
    @include desktop {
      line-height: 30px;
      font-size: 20px;
      max-width: 590px;
    }
  }
  &__button {
    width: 240px;
    height: 48px;
    background: linear-gradient(134.79deg, #63e1d9 -42.11%, #34a0cd 100%);
    box-shadow: 2px 3px 6px rgba(0, 0, 0, 0.15925);
    border: none;
    border-radius: 24px;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 14px;
    line-height: 16px;
    color: #ffffff;
    @include desktop {
      width: 280px;
      height: 56px;
      background: linear-gradient(138.1deg, #63e1d9 -49.34%, #34a0cd 100%);
      border-radius: 28px;
      font-size: 16px;
      line-height: 19px;
    }
  }
}
</style>
