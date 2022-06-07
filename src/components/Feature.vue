<template>
  <div className="feature__container">
    <slot></slot>
  </div>
</template>

<script></script>

<style lang="scss">
@use '../styles/mixins.scss' as *;

.feature {
  &__container {
    margin-bottom: 80px;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0 28px;
    &:last-child {
      margin-bottom: 0;
    }
    @include desktop {
      padding: 0;
      margin: 0;
    }
  }
  &__image {
    margin-bottom: 24px;
    height: 80px;
    width: auto;
    @include desktop {
      height: 104px;
      margin-bottom: 1rem;
    }
  }
  &__header {
    margin-bottom: 0.5rem;
    font-family: 'Raleway';
    font-style: normal;
    font-weight: 700;
    font-size: 18px;
    line-height: 24px;
    text-align: center;
    color: #ffffff;
    @include desktop {
      font-size: 20px;
      line-height: 23px;
    }
  }
  &__text {
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    color: #ffffff;
    @include desktop {
      font-size: 14px;
      line-height: 21px;
      max-width: 350px;
    }
  }
}
</style>
