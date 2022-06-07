<template>
  <div className="testimonial__container">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'Testimonial',
};
</script>

<style lang="scss">
@use '../styles/mixins.scss' as *;

.testimonial {
  &__container {
    margin-bottom: 24px;
    background: #202a3c;
    box-shadow: 0px 0px 8px 4px rgba(56, 56, 56, 0.0458843);
    border-radius: 3.93258px;
    padding: 20px 24px 20px 21px;
    position: relative;
    z-index: 2;
    &:last-child {
      margin: 0;
    }
    @include desktop {
      margin: 0;
      margin-right: 40px;
      padding: 40px 25px 26px 26px;
    }
  }
  &__quote {
    margin-bottom: 16px;
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 10px;
    line-height: 18px;
    color: #ffffff;
    letter-spacing: 0.5px;
    @include desktop {
      font-size: 14px;
      line-height: 21px;
    }
  }
  &__author-container {
    display: flex;
  }
  &__author-image {
    margin-right: 8px;
    border-radius: 50%;
    width: 24px;
    height: 24px;
  }
  &__author-name {
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 700;
    font-size: 10px;
    line-height: 12px;
    letter-spacing: 0.5px;
    color: #ffffff;
    margin-bottom: 4px;
  }
  &__author-title {
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 7px;
    line-height: 10px;
    letter-spacing: 0.5px;
    color: #ffffff;
  }
}
</style>
