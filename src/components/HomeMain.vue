<script>
</script>

<template>
  <!-- First Section -->
  <section class="ms_first-section">
    <div class="ms_wrapper">
      <div class="ms_section-title text-center">
        <h5>start learning coding languages</h5>
        <h2>Build Your Dream <span>TODAY</span></h2>
      </div>
      <div class="row row-cols-1 row-cols-md-4 g-4">
        <div class="col">
          <div class="card h-100">
            <img src="../assets/images/home-5-image-box-01.png" class="card-img-top" alt="Group of people at a table">
            <div class="card-body text-center">
              <h5 class="card-title">Idea Discussion</h5>
              <p class="card-text">Get teamed up with the specialists who work and teach coding for years at famous
                universities.</p>
              <a href="#">
                <h6>Start now &#8594;</h6>
              </a>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <img src="../assets/images/home-5-image-box-02.png" class="card-img-top" alt="Guy analyzing code">
            <div class="card-body text-center">
              <h5 class="card-title">Web Development</h5>
              <p class="card-text">Learn to start building a webpage from scratch. You decide your own pace, course
                and
                speed.</p>
              <a href="#">
                <h6>Start now &#8594;</h6>
              </a>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <img src="../assets/images/home-5-image-box-03.png" class="card-img-top" alt="Two people analyzing a graph">
            <div class="card-body text-center">
              <h5 class="card-title">System Administration</h5>
              <p class="card-text">Learners are encouraged to study the mechanism and structure of system
                administration.
              </p>
              <a href="#">
                <h6>Start now &#8594;</h6>
              </a>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <img src="../assets/images/home-5-image-box-04.png" class="card-img-top"
              alt="A person designing a dashboard">
            <div class="card-body text-center">
              <h5 class="card-title">Graphic Design</h5>
              <p class="card-text">Have a passion for graphic and arts? Show your talents with confidence and
                self-assertiveness.</p>
              <a href="#">
                <h6>Start now &#8594;</h6>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

// First Section
.ms_first-section {
  background-color: $secondary--background;

  .ms_section-title {
    padding: 100px 0;

    h5 {
      color: $primary_cod-gray;
      text-transform: uppercase;
    }

    h2 {
      font-size: 50px;
      font-weight: 600;
      padding-top: 20px;
      color: $primary_mulled-wine;

      span {
        font-weight: 500;
        color: $third_jungle-green;
      }
    }
  }

  .card {
    background-color: $secondary--background;
    padding-bottom: 100px;
    display: flex;
    align-items: center;
    --bs-card-spacer: 0;
    --bs-card-border-color: none;

    a {
      text-decoration: none;
    }

    h6 {
      padding-top: 30px;
      font-size: 16px;
      font-weight: 700;
      color: rgba($primary_mulled-wine , $alpha: .7);
      transition: 0.3s;

      &:hover {
        color: $third_jungle-green;
        transition: 0.3s;
      }
    }

    h5 {
      padding-top: 10px;
      color: $primary_cod-gray;
      font-size: 22px;
      font-weight: 700;
    }

    p {
      padding-top: 10px;
    }

    img {
      width: 150px;
      height: 150px;
      object-fit: contain;
    }
  }
}
</style>
