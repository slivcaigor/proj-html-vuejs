<script>
export default {
  data() {
    return {
      // used to control the visibility of the button
      showBackToTop: false,
      linksFirstCol: [
        {
          heading: 'Explore',
        },
        {
          text: 'Start here',
          url: '#',
        },
        {
          text: 'Blog',
          url: '#',
        },
        {
          text: 'About us',
          url: '#',
        },
      ],
      linksSecondCol: [
        {
          heading: 'Explore',
        },
        {
          text: 'Success story',
          url: '#',
        },
        {
          text: 'Courses',
          url: '#',
        },
        {
          text: 'Contact us',
          url: '#',
        },
      ],
      linksThirdCol: [
        {
          heading: 'Information',
        },
        {
          text: 'Membership',
          url: '#',
        },
        {
          text: 'Purchase guide',
          url: '#',
        },
        {
          text: 'Privacy policy',
          url: '#',
        },
        {
          text: 'Terms of services',
          url: '#',
        },
      ],
      linksFourthCol: [
        {
          heading: 'Address',
        },
        {
          address: '382 NE 191st St # 87394 Miami, FL 33179-3899',
        },
        {
          contacts: '+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)',
        },
        {
          email: 'support@maxcoach.com',
        },
      ],
    };
  },
  // a method called scrollToTop that uses window.scrollTo to scroll the window to the top of the page
  methods: {
    scrollToTop() {
      window.scrollTo(0, 0);
    },
  },
  // listens for the scroll event and updates the value of showBackToTop based on the scroll position
  mounted() {
    window.addEventListener('scroll', () => {
      this.showBackToTop = window.scrollY > 0;
    });
  },
};
</script>

<template>
  <section>
    <div class="ms_wrapper">
      <div class="ms_footer d-flex justify-content-between">
        <div class="ms_address">
          <ul>
            <li v-for="(link, index) in linksFourthCol" :key="index">
              <h5>{{ link.heading }}</h5>
              <h6>{{ link.address }}</h6>
              <h6>{{ link.contacts }}</h6>
              <h6>{{ link.email }}</h6>
            </li>
          </ul>
          <div class="ms_socials">
            <a href="#"><img src="../assets/icons/facebook.png" alt="Facebook Logo"></a>
            <a href="#"><img src="../assets/icons/twitter.png" alt="Twitter Logo"></a>
            <a href="#"><img src="../assets/icons/instagram.png" alt="Instagram Logo"></a>
            <a href="#"><img src="../assets/icons/linkedin.png" alt="LinkedIn Logo"></a>
          </div>
        </div>
        <div class="ms_footer-nav">
          <div class="col">
            <ul>
              <li v-for="(link, index) in linksFirstCol" :key="index">
                <h5>{{ link.heading }}</h5>
                <a :href="link.url">
                  {{ link.text }}
                </a>
              </li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li v-for="(link, index) in linksSecondCol" :key="index">
                <h5>{{ link.heading }}</h5>
                <a :href="link.url">
                  {{ link.text }}
                </a>
              </li>
            </ul>
          </div>
          <div class="col">
            <ul>
              <li v-for="(link, index) in linksThirdCol" :key="index">
                <h5>{{ link.heading }}</h5>
                <a :href="link.url">
                  {{ link.text }}
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="ms_copyright text-center">
        &#169; 2020 Maxcoach. All Rights Reserved
      </div>
    </div>
    <!-- control the visibility of the button based on the value of showBackToTop -->
    <div v-if="showBackToTop" @click="scrollToTop" class="ms_top-page-btn">&#8593;</div>
  </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;


section {
  position: relative;

  .ms_top-page-btn {
    z-index: 666;
    position: fixed;
    bottom: 30px;
    right: 30px;
    cursor: pointer;
    background-color: $third_jungle-green;
    color: white;
    font-size: 40px;
    padding: 20px;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .ms_copyright {
    padding: 100px 0 50px;
    color: rgba($color: #000000, $alpha: .6);
  }

  .ms_footer-nav {
    padding-top: 50px;
    padding-right: 150px;
    display: flex;
    gap: 70px;

    .col {
      h5 {
        padding-bottom: 10px;
      }

      &:nth-of-type(2) {
        h5 {
          color: transparent;
        }
      }
    }

    h5 {
      color: black;
      font-weight: 600;
    }

    li {
      width: max-content;

      a {
        text-decoration: none;
        color: rgba($color: #000000, $alpha: .5);
        font-size: 15px;
        font-weight: 600;
      }
    }
  }

  .ms_address {
    padding-top: 50px;

    .ms_socials {
      padding-top: 20px;

      img {
        padding-right: 20px;
      }
    }

    h5 {
      color: black;
      font-weight: 600;

      &:first-child {
        padding-bottom: 5px;
      }
    }

    h6 {
      font-size: 16px;
      color: rgba($color: #000000, $alpha: .7);

      &:nth-of-type(2) {
        padding: 5px 0;
      }
    }
  }
}
</style>
