<template>
  <section id="info-footer">
    <div class="adava-info container">
      <!-- Social  -->
      <div class="col social-info">
        <a href="#">
          <img src="@/assets/images/medical_logo_1x_dark.png" alt="adava" />
        </a>
        <p>
          Sed ut perspiciatis unde omnis iste natus error sit voluptatem
          accusantium dolemue launti totam aperiam, eaque ipsa quae abillo.
          Invente veriatis et quasi architecto beatae luptatem accusantium,
          remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem
          ipsum sits dolores ets unser.
        </p>
        <span class="uppercase">learn more about us</span>
        <div class="social-icon">
          <a href="#">
            <i
              v-for="(social, index) in socialClass"
              :key="index"
              class="fab"
              :class="social"
            ></i>
          </a>
        </div>
      </div>
      <!-- Contact  -->
      <div class="col contact-info">
        <h6 class="uppercase">contact information</h6>
        <div>
          <i class="fas fa-map-marker-alt"></i>
          <address>121king Street, London United Kingdom</address>
        </div>
        <div>
          <i class="fas fa-phone"></i>
          <span>1.800.458.556</span>
        </div>
      </div>
      <!-- Departments -->
      <div class="col departments-info">
        <h6 class="uppercase">medical depaertments</h6>
        <ul>
          <li v-for="(department, index) in departments" :key="index">
            <a href="#">{{ department }}</a>
          </li>
        </ul>
      </div>
    </div>
    <div class="copyright"></div>
  </section>
</template>

<script>
export default {
  name: "InfoFooter",
  props: ["departments"],
  data() {
    return {
      socialClass: [
        "fa-facebook-square",
        "fa-twitter-square",
        "fa-youtube-square",
        "fa-instagram-square",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
//// Import variables
@import "../scss/General/_vars.scss";

//// General style
#info-footer {
  padding: 40px 0;
}
.adava-info {
  display: flex;
  align-items: center;
}
.contact-info,
.departments-info {
  width: 350px;
}

//// Style social info section
.social-info {
  width: 500px;
  img {
    width: 200px;
    margin-bottom: 10px;
  }
  p {
    font-size: 12px;
    width: 420px;
    font-weight: lighter;
    line-height: 24px;
    color: $grey;
    &::after {
      content: "";
      width: 420px;
      border: 0.1px solid $light-grey;
      display: inline-block;
    }
  }
  span {
    font-size: 12px;
    font-weight: lighter;
    color: $dark-grey;
  }
  .social-icon {
    margin-top: 20px;
    font-size: 22px;
    i {
      padding-right: 5px;
      &.fa-facebook-square {
        color: $fb-color;
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-twitter-square {
        color: $twitter-color;
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-youtube-square {
        color: $youtube-color;
        &:hover {
          transform: scale(1.1);
        }
      }
      &.fa-instagram-square {
        color: $insta-color;
        &:hover {
          transform: scale(1.1);
        }
      }
    }
  }
}
</style>