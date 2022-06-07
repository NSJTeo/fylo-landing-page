<template>
  <div className="info__container">
    <img
      className="info__image"
      src="../assets/illustrations/illustration-stay-productive.png"
      alt=""
    />
    <div>
      <p className="info__header">Stay productive, wherever you are</p>
      <p className="info__text">
        Never let location be an issue when accessing your files. Fylo has you
        covered for all of your file storage needs.
      </p>
      <p className="info__text">
        Securely share files and folders with friends, family and colleagues for
        live collaboration. No email attachments required.
      </p>
      <div className="info__link">
        <p className="info__link-text">See how Fylo works</p>
        <img
          className="info__link-image"
          src="../assets/icons/icon-arrow.svg"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Info',
};
</script>

<style lang="scss">
@use '../styles/mixins.scss' as *;

.info {
  &__container {
    max-width: 1440px;
    padding: 0 28px;
    padding-bottom: 160px;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 0 auto;
    @include info {
      flex-direction: row;
      padding: 0 101px 179px 105px;
    }
  }
  &__image {
    margin-bottom: 48px;
    width: 100%;
    max-width: 615px;
    @include info {
      margin: 0;
      margin-right: 57px;
      width: 50%;
    }
  }
  &__header {
    margin-bottom: 1rem;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 24px;
    text-align: center;
    color: #ffffff;
    @include info {
      font-size: 40px;
      line-height: 50px;
      margin-bottom: 19px;
      text-align: start;
      max-width: 478px;
    }
  }
  &__text {
    margin-bottom: 1rem;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    color: #ffffff;
    max-width: 563px;
    @include info {
      font-size: 16px;
      line-height: 24px;
    }
  }
  &__link {
    padding-bottom: 6px;
    border-bottom: 1px solid #62e0d9;
    width: fit-content;
    display: flex;
    align-items: center;
    @include info {
      margin-top: 24px;
    }
  }
  &__link-text {
    margin-right: 7px;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 16px;
    color: #62e0d9;
  }
  &__link-image {
    width: 12px;
    height: 12px;
  }
}
</style>
