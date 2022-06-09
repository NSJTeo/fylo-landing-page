<template>
  <footer className="footer__background">
    <div className="footer__container">
      <img className="footer__logo" src="../assets/misc/logo.svg" alt="" />
      <div class="footer__inner-container">
        <div className="footer__contact-container">
          <div
            class="footer__contact-inner-container footer__contact-inner-container--location"
          >
            <div
              class="footer__contact-icon-container footer__contact-icon-container--location"
            >
              <img src="../assets/icons/icon-location.svg" alt="" />
            </div>
            <p className="footer__contact-info footer__contact-info--location">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua
            </p>
          </div>
          <div class="footer__phone-email-container">
            <div class="footer__contact-inner-container">
              <div class="footer__contact-icon-container">
                <img src="../assets/icons/icon-phone.svg" alt="" />
              </div>
              <p className="footer__contact-info">+1-543-123-4567</p>
            </div>
            <div class="footer__contact-inner-container">
              <div class="footer__contact-icon-container">
                <img src="../assets/icons/icon-email.svg" alt="" />
              </div>
              <p className="footer__contact-info">example@fylo.com</p>
            </div>
          </div>
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
@use '../styles/mixins.scss' as *;

.footer {
  &__background {
    background: $background-footer;
  }
  &__container {
    padding: 0 28px;
    padding-bottom: 52px;
    padding-top: 259px;
    max-width: 1440px;
    margin: 0 auto;
  }
  &__inner-container {
    @include footer {
      display: flex;
    }
  }
  &__logo {
    width: 108px;
    height: auto;
    margin-left: 11px;
    margin-bottom: 35px;
  }
  &__contact-container {
    display: flex;
    flex-direction: column;
    margin-bottom: 56px;
    @include footer {
      margin-bottom: 0;
      flex-direction: row;
    }
  }
  &__phone-email-container {
    @include footer {
      margin-right: 146px;
    }
  }
  &__contact-icon-container {
    min-width: 28px;
    height: 28px;
    display: flex;
    align-items: center;
    margin-right: 1rem;
    &--location {
      padding-top: 2px;
    }
  }
  &__contact-inner-container {
    display: flex;
    margin-bottom: 1rem;
    align-items: center;
    &:first-child {
      align-items: flex-start;
    }
    &:last-child {
      margin: 0;
    }
    &--location {
      margin-right: 80px;
    }
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
      @include footer {
        max-width: 339px;
      }
    }
    &:last-child {
      margin-bottom: 0;
    }
  }
  &__links {
    display: flex;
  }
  &__left-links {
    margin-bottom: 48px;
    @include footer {
      margin-bottom: 0;
      margin-right: 80px;
    }
  }
  &__right-links {
    margin-bottom: 56px;
    @include footer {
      margin-bottom: 0;
    }
  }
  &__link {
    margin-bottom: 1rem;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 22px;
    color: #ffffff;
    cursor: pointer;
    &:last-child {
      margin-bottom: 0;
    }
    &:hover {
      font-weight: 700;
    }
  }
  &__social-media-links {
    display: flex;
    justify-content: center;
    @include footer {
      margin-left: auto;
    }
  }
  &__social-media-link {
    margin-right: 10.82px;
    height: 31px;
    width: auto;
    cursor: pointer;
    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
