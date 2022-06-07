<template>
  <div className="feature__container">
    <slot></slot>
  </div>
</template>

<script></script>

<style lang="scss">
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
  }
  &__image {
    margin-bottom: 24px;
    height: 80px;
    width: auto;
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
  }
  &__text {
    font-family: 'Open Sans';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    color: #ffffff;
  }
}
</style>
