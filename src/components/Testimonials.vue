<template>
  <div className="testimonials__container">
    <div className="testimonials__inner-container">
      <img
        className="testimonials__icon"
        src="../assets/backgrounds/bg-quotes.png"
        alt=""
      />
      <Testimonial v-for="testimonial in testimonials" :key="testimonial.id">
        <p className="testimonial__quote">{{ testimonial.quote }}</p>
        <div className="testimonial__author-container">
          <img :src="testimonial.image" className="testimonial__author-image" />
          <div>
            <p className="testimonial__author-name">{{ testimonial.name }}</p>
            <p className="testimonial__author-title">{{ testimonial.title }}</p>
          </div>
        </div>
      </Testimonial>
    </div>
  </div>
</template>

<script>
import Testimonial from './Testimonial.vue';
import testimonials from '../assets/data/testimonials.json';
import profilePic1 from '../assets/profiles/profile-1.jpg';
import profilePic2 from '../assets/profiles/profile-2.jpg';
import profilePic3 from '../assets/profiles/profile-3.jpg';

const profilePics = [profilePic1, profilePic2, profilePic3];
testimonials.forEach((testimonial, i) => (testimonial.image = profilePics[i]));

export default {
  name: 'Testimonials',
  components: { Testimonial },
  data() {
    return {
      testimonials,
    };
  },
};
</script>

<style lang="scss">
@use '../styles/mixins.scss' as *;

.testimonials {
  &__container {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0 48px;
    max-width: 1180px;
    margin: 0 auto;
  }
  &__inner-container {
    position: relative;
    @include desktop {
      display: flex;
      padding-left: 20px;
      justify-content: center;
    }
  }
  &__icon {
    position: absolute;
    width: 28px;
    height: auto;
    top: -19px;
    left: 8px;
    z-index: 1;
    @include desktop {
      width: 75px;
      top: -45px;
    }
  }
}
</style>
