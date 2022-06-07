<template>
  <div className="features__background">
    <div className="features__container">
      <Feature v-for="feature in features" :key="feature.id">
        <img :src="feature.image" className="feature__image" />
        <p className="feature__header">{{ feature.header }}</p>
        <p className="feature__text">{{ feature.text }}</p>
      </Feature>
    </div>
  </div>
</template>

<script>
import features from '../assets/data/features.json';
import Feature from './Feature.vue';
import anywhereIcon from '../assets/icons/icon-access-anywhere.svg';
import securityIcon from '../assets/icons/icon-security.svg';
import collaborationIcon from '../assets/icons/icon-collaboration.svg';
import anyFileIcon from '../assets/icons/icon-any-file.svg';

const images = [anywhereIcon, securityIcon, collaborationIcon, anyFileIcon];

features.forEach((feature, i) => {
  feature.image = images[i];
});

export default {
  name: 'Features',
  components: { Feature },
  data() {
    return {
      features,
    };
  },
};
</script>

<style lang="scss">
@use '../styles/mixins.scss' as *;

.features {
  &__background {
    margin-top: 120px;
    margin-bottom: 160px;
    @include desktop {
      margin-top: 158px;
      margin-bottom: 138px;
    }
  }
  &__container {
    max-width: 880px;
    display: flex;
    flex-direction: column;
    align-items: center;
    @include desktop {
      display: grid;
      grid-template-columns: 1fr 1fr;
      row-gap: 78px;
      margin: 0 auto;
    }
  }
}
</style>
