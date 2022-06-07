<template>
  <footer className="footer__background">
    <div className="footer__container">
      <img className="footer__logo" src="../assets/misc/logo.svg" alt="" />
      <div className="footer__contact-container">
        <img
          className="footer__contact-icon"
          src="../assets/icons/icon-location.svg"
          alt=""
        />
        <p className="footer__contact-info footer__contact-info--location">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua
        </p>
        <img
          className="footer__contact-icon"
          src="../assets/icons/icon-phone.svg"
          alt=""
        />
        <p className="footer__contact-info">+1-543-123-4567</p>
        <img
          className="footer__contact-icon"
          src="../assets/icons/icon-email.svg"
          alt=""
        />
        <p className="footer__contact-info">example@fylo.com</p>
      </div>
      <div className="footer__left-links">
        <p className="footer__link">About Us</p>
        <p className="footer__link">Jobs</p>
        <p className="footer__link">Press</p>
        <p className="footer__link">Blog</p>
      </div>
      <div className="footer__right-links">
        <p className="footer__link">Contact Us</p>
        <p className="footer__link">Terms</p>
        <p className="footer__link">Privacy</p>
      </div>
      <div className="footer__social-media-links">
        <img
          className="footer__social-media-link"
          src="../assets/icons/icon-facebook.svg"
          alt=""
        />
        <img
          className="footer__social-media-link"
          src="../assets/icons/icon-twitter.svg"
          alt=""
        />
        <img
          className="footer__social-media-link"
          src="../assets/icons/icon-instagram.svg"
          alt=""
        />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
@use '../styles/variables.scss' as *;

.footer {
  &__background {
    background: $background-footer;
  }
  &__container {
    padding: 0 28px;
    padding-bottom: 52px;
  }
  &__logo {
    width: 108px;
    height: auto;
    margin-left: 11px;
    margin-bottom: 35px;
  }
  &__contact-container {
    display: grid;
    grid-template-columns: 40px 1fr;
    margin-bottom: 56px;
  }
  &__contact-icon {
    margin-right: 1rem;
  }
  &__contact-info {
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    color: #ffffff;
    margin-bottom: 19px;
    &--location {
      font-size: 16px;
      line-height: 24px;
      margin-bottom: 16px;
    }
    &:last-child {
      margin-bottom: 0;
    }
  }
  &__left-links {
    margin-bottom: 48px;
  }
  &__right-links {
    margin-bottom: 56px;
  }
  &__link {
    margin-bottom: 1rem;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 22px;
    color: #ffffff;
    &:last-child {
      margin-bottom: 0;
    }
  }
  &__social-media-links {
    display: flex;
    justify-content: center;
  }
  &__social-media-link {
    margin-right: 10.82px;
    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
