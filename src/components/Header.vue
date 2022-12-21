<script>
export default {
  data() {
    return {
      links: [
        {
          text: 'Home',
          url: '#',
        },
        {
          text: 'Pages',
          url: '#',
        },
        {
          text: 'Courses',
          url: '#',
        },
        {
          text: 'Features',
          url: '#',
        },
        {
          text: 'Blog',
          url: '#',
        },
        {
          text: 'Shop',
          url: '#',
        },
      ],
    }
  }
}
</script>

<template>
  <div class="ms_container">
    <div class="ms_hero-wave">
      <img src="../assets/images/jumbo-overlay.svg" alt="Wave Hero Overlay">
    </div>
    <div class="ms_sidenav">
      <img src="../assets/icons/ruler.png" alt="Ruler Icon">
      <img src="../assets/icons/lifeguard.png" alt="Lifeguard Ring Icon">
      <img src="../assets/icons/book.png" alt="Book Icon">
      <img src="../assets/icons/shopping-cart.png" alt="Shopping Cart Icon">
    </div>
    <div class="ms_wrapper">
      <!-- Top Main Navigation -->
      <div class="ms_nav px-3 py-3 d-flex align-items-center">
        <!-- Logo -->
        <div class="ms_logo">
          <img src="../assets/images/dark-logo.png" alt="MaxCoach Logo">
        </div>
        <!-- Menu Voices -->
        <div class="ms_navigation">
          <nav>
            <ul class="d-flex align-items-center">
              <!-- v-for loop that iterates over an array of objects called links -->
              <li class="ms_nav-link" v-for="(link, index) in links" :key="index">
                <!-- For each object in the links array, it creates a <li> element that contains an <a> element -->
                <a href="#">
                  {{ link.text }}
                  <img src="../assets/icons/chevron-down.png" alt="Arrow Dropdown Menu">
                </a>
              </li>
              <li class="ms_nav-link">
                <a href="#">
                  <span id="ms_shopping-cart">
                    <img id="ms_cart-icon" src="../assets/icons/shopping-cart.png" alt="Shopping Cart">
                    <span class="label">0</span>
                  </span>
                </a>
                <a href="#">
                  <img id="ms_user-avatar" src="../assets/icons/user-profile.png" alt="User Profile Avatar">
                </a>
              </li>
            </ul>
          </nav>
        </div>
        <!-- Search Bar -->
        <div class="ms_search-bar">
          <form class="ms_search-form">
            <input type="text" class="ms_search-input" placeholder="Search...">
            <img class="ms_search-icon" src="../assets/icons/search.png" alt="Search Icon">
          </form>
        </div>
      </div>
      <!-- Hero Section -->
      <div class="row mt-5 justify-content-between ms_index position-relative">
        <!-- Hero Text -->
        <div class="col-6 ms_hero-text">
          <h1>Complete Your Dreams in JavaS Programming</h1>
          <p>
            Learn any coding program in distance and for a reasonable fee. You don't have to struggle alone, you've got
            our assistance and help.
          </p>
          <button>
            <img src="../assets/icons/download.png" alt="Download Icon">
            <span>Download free E-book</span>
          </button>
        </div>
        <!-- Hero Image -->
        <div class="col-6">
          <img src="../assets/images/home-5-hero-image.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

.ms_index {
  z-index: 555;
}

.ms_hero-text {
  width: 40%;
  padding: 4.063em 1.563em;

  h1 {
    font-size: 3.125rem;
    font-weight: 600;
    color: $primary_mulled-wine;
  }

  p {
    font-size: 18px;
    padding: 1.875em 0 2.5em 0;
    color: rgba($primary_mulled-wine, $alpha: .7);
    font-weight: 600;
  }

  button {
    background-color: $third_jungle-green;
    border: none;
    padding: 0.813em 0;
    border-radius: 0.313em;
    width: 60%;

    img {
      width: 1.875rem;
      padding-right: 0.438em;
    }

    span {
      vertical-align: middle;
      font-size: 1rem;
      font-weight: 700;
      color: $primary_white;
    }
  }
}

.ms_search-bar {
  width: 16.5%;

  .ms_search-form {
    height: 3.125em;
    position: relative;

    .ms_search-input {
      border: none;
      border-radius: 5px;
      height: 100%;
      padding: 0 2.5em 0.313em 1.25em;
      width: 100%;
    }

    .ms_search-icon {
      position: absolute;
      width: 1.875rem;
      right: 0.625rem;
      top: 50%;
      transform: translateY(-50%);
    }
  }
}

.ms_container {
  background-color: $primary--background;
  padding-bottom: 3.75em;
  overflow: hidden;
  position: relative;

  .ms_sidenav {
    background-color: $primary_white;
    position: absolute;
    top: 36%;
    left: 99%;
    transform: translate(-50%, -50%);
    width: 2.5rem;
    height: 10rem;
    border-radius: 0.313rem 0 0 0.313rem;
    box-shadow: 0 0 0.313rem 0 $third_oslo-gray;
    display: flex;
    flex-direction: column;
    gap: 0.938em;
    align-items: center;
    justify-content: space-evenly;
    padding: 0.125em;

    img {
      cursor: pointer;
      width: 45%;
    }
  }

  .ms_hero-wave {
    img {
      z-index: 1;
      position: absolute;
      height: 55%;
      width: 100%;
      left: 0;
      bottom: 0;
      right: 0;
      transform: rotateX(180deg);
    }
  }

  .ms_logo {
    width: 13.5%;
    margin-right: auto;
  }

  .ms_navigation {

    #ms_shopping-cart {
      position: relative;

      #ms_cart-icon {
        width: 1.375rem;
        margin-left: 0.313em;
        padding: 0;
      }

      .label {
        background-color: $third_jungle-green;
        border-radius: 50%;
        color: $primary_white;
        font-size: 12px;
        font-weight: bold;
        position: absolute;
        right: -0.5rem;
        top: -0.375rem;
        padding: 0 0.375em;
      }
    }

    .ms_nav-link {

      &:nth-last-child(n+2) {
        padding-left: 2.688em;
      }

      #ms_user-avatar {
        width: 1.25rem;
        margin-left: 1.875em;
        margin-right: 0.938em;
      }

      a {
        color: $primary_mulled-wine;
        font-weight: 600;
      }

      img {
        width: 0.5rem;
      }
    }
  }
}
</style>

