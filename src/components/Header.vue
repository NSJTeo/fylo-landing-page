<template>
  <header className="header__background">
    <div className="header__container">
      <img className="header__logo" src="../assets/misc/logo.svg" alt="" />
      <div className="header__links">
        <p className="header__link">Features</p>
        <p className="header__link">Team</p>
        <p className="header__link">Sign In</p>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style lang="scss">
@use '../styles/variables.scss' as *;
@use '../styles/mixins.scss' as *;

.header {
  &__background {
    background: $background-secondary;
  }
  &__container {
    max-width: 1440px;
    padding: 24px 20px;
    padding-bottom: 0;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    @include desktop {
      padding: 73px 80px 0 80px;
    }
  }
  &__logo {
    height: 24px;
    width: auto;
    @include desktop {
      height: 52px;
    }
  }
  &__links {
    display: flex;
    align-items: center;
  }
  &__link {
    margin-right: 24px;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 14px;
    color: #ffffff;
    cursor: pointer;
    &:last-child {
      margin: 0;
    }
    @include desktop {
      font-size: 16px;
      line-height: 19px;
      margin-right: 58px;
    }
    &:hover {
      text-decoration-line: underline;
      font-weight: 700;
    }
  }
}
</style>
