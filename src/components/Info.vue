<template>
  <div className="info__container">
    <img
      className="info__image"
      src="../assets/illustrations/illustration-stay-productive.png"
      alt=""
    />
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
</template>

<script>
export default {
  name: 'Info',
};
</script>

<style lang="scss">
.info {
  &__container {
    max-width: 1440px;
    padding: 0 28px;
    padding-bottom: 160px;
  }
  &__image {
    margin-bottom: 48px;
    width: 100%;
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
  }
  &__text {
    margin-bottom: 1rem;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    color: #ffffff;
  }
  &__link {
    padding-bottom: 6px;
    border-bottom: 1px solid #62e0d9;
    width: fit-content;
    display: flex;
    align-items: center;
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
