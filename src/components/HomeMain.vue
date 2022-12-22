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
  <!-- Second Section -->
  <section class="ms_second-section">
    <div class="ms_wrapper">
      <div class="row mt-5 justify-content-between ms_index position-relative">
        <div class="col-6">
          <img src="../assets/images/underlay-shape-lilla.svg" alt="Lilla Colored Shape">
          <img src="../assets/images/about-us-03-image-01.png" alt="Guy cheering over laptop screen">
        </div>
        <div class="col-6 ms_hero-text">
          <h5>dream with <strong>maxcoach</strong></h5>
          <h2 class="ms_section-heading">Construct A <span>Stunning</span> Career Perspective</h2>

          <div class="accordion" id="accordionExample">
            <div class="accordion-item">
              <h2 class="accordion-header" id="headingOne">
                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne"
                  aria-expanded="true" aria-controls="collapseOne">
                  Multiple Platforms Supported for Teaching & Studying
                </button>
              </h2>
              <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne"
                data-bs-parent="#accordionExample">
                <div class="accordion-body">
                  MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via
                  material downloads. We know things aren't supposed to be devoured in a short time, you can always
                  access our knowledge from any device.
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <h2 class="accordion-header" id="headingTwo">
                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                  data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                  Multiple Course Participation at the Same Time
                </button>
              </h2>
              <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo"
                data-bs-parent="#accordionExample">
                <div class="accordion-body">
                  MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via
                  material downloads. We know things aren't supposed to be devoured in a short time, you can always
                  access our knowledge from any device.
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <h2 class="accordion-header" id="headingThree">
                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                  data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                  Track Study Progress & Deliver Prompt Feedback
                </button>
              </h2>
              <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree"
                data-bs-parent="#accordionExample">
                <div class="accordion-body">
                  MaxCoach supports the act of teaching and learning on multiple platforms like online or offline via
                  material downloads. We know things aren't supposed to be devoured in a short time, you can always
                  access our knowledge from any device.
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Third Section -->
  <section class="ms_third-section">
    <div class="ms_wrapper">
      <div class="d-flex justify-content-around align-items-center text-center">
        <div>
          <h4>1.926</h4>
          <h5>finished sessions</h5>
        </div>
        <div>
          <h4>3.092+</h4>
          <h5>enrolled learners</h5>
        </div>
        <div>
          <h4>200</h4>
          <h5>online instructors</h5>
        </div>
        <div>
          <h4>100%</h4>
          <h5>satisfaction rate</h5>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

// Third Section
.ms_third-section {
  background-color: #FAF8F6;
  padding: 100px 0;

  h4 {
    color: $secondary_jungle-green;
    font-weight: 900;
    font-size: 50px;
  }

  h5 {
    color: $primary_mulled-wine;
    font-weight: 600;
    font-size: 18px;
    text-transform: uppercase;
  }
}

// Second Section
.ms_second-section {
  padding-top: 50px;
  background-color: $secondary--background;
  padding-bottom: 100px;

  .col-6 {
    img:first-child {
      position: absolute;
      z-index: 1;
      width: 30%;
      left: -100px;
      bottom: 70px;
    }

    img:last-child {
      position: relative;
      z-index: 2;
    }
  }

  .ms_hero-text {
    .accordion {
      --bs-accordion-btn-focus-box-shadow: #62C5B5;
      --bs-accordion-btn-focus-border-color: #62C5B5;
    }

    #accordionExample {
      --bs-accordion-border-color: none;
      --bs-accordion-active-color: $primary_white;
      --bs-accordion-btn-icon: url("../assets/icons/add.png");
      --bs-accordion-btn-active-icon: url("../assets/icons/minus.png");
      --bs-accordion-btn-icon-width: 1.7rem;

      .accordion-item {
        border-radius: 5px;
        box-shadow: 0 0 10px 0 rgba($third_gray, $alpha: .3);
        background-color: $primary_white;

        &:nth-child(2) {
          margin: 30px 0;
        }

        .accordion-button {
          font-weight: 700;
          font-size: 16px;
          color: rgba($primary_black, $alpha: .6);
          border-radius: 5px;
        }

        .accordion-button:not(.collapsed) {
          color: rgba($color: $primary_white, $alpha: 1);
          background-color: $shadow;
          border-bottom-right-radius: 0;
          border-bottom-left-radius: 0;
        }
      }
    }

    h5 {
      color: $primary_cod-gray;
      text-transform: uppercase;
      font-size: 18px;
    }

    .ms_section-heading {
      font-size: 50px;
      font-weight: 600;
      padding: 20px 0 40px 0;
      color: $primary_mulled-wine;

      span {
        font-weight: 500;
        color: $third_jungle-green;
      }
    }
  }
}

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
