<template>
    <main>

      <!-- "Start Investing" Section -->
      <section>
        <div class="container-sm">
          <div class="colums-wrapper">

            <!-- Column Left -->
            <div class="col-left">
              
              <!-- Title -->
              <h2>
                Start Investing in You
              </h2>

              <!-- Subtitle -->
              <h3>
                With over 1200 courses in 18 subjects, you're guaranteed to find something that's right for you.
              </h3>

              <!-- Sign Up Button -->
              <a href="#" class="btn">
                  join for free
              </a>
            </div>

            <!-- Column Right -->
            <div class="col-right">

              <!-- Background Image -->
              <img class="bg-img" src="../assets/img/base.png" alt="base">

              <!-- Moon Image -->
              <img class="moon-img" src="../assets/img/moon.png" alt="moon">

              <!-- Bubblespeech Image -->
              <img class="bubblespeech-img" src="../assets/img/bubblespeech.png" alt="bubblespeech">

              <!-- Book 1 Image -->
              <img class="book1-img" src="../assets/img/book1.png" alt="book1">

              <!-- Book 2 Image -->
              <img class="book2-img" src="../assets/img/book2.png" alt="book2">

              <!-- Magnifier Image -->
              <img class="magnifier-img" src="../assets/img/magnifier.png" alt="magnifier">
            </div>
          </div>

            <!-- Benefits -->
            <div class="benefits">

              <!-- "Worldwide Recognize" -->
              <div class="col-benefits">

                <!-- Icon -->
                <div>
                  <i class="fa-solid fa-earth-africa"></i>
                </div>

                <!-- Title -->
                <h4>
                  Worldwide Recognize
                </h4>

                <!-- Text -->
                <div class="text-benefits">
                  Our online course certificates can be used around the world and also in most popular universities and companies.
                </div>
              </div>

              <!-- "Mostly Online Learning" -->
              <div class="col-benefits">

                <!-- Icon -->
                <div>
                  <i class="fa-solid fa-desktop"></i>
                </div>

                <!-- Title -->
                <h4>
                  Mostly Online Learning (sd)
                </h4>

                <!-- Text -->
                <div class="text-benefits">
                  Masterstudy online certificates can be obtained in a range of specialized areas and typically take about a year to complete.
                </div>
              </div>

              <!-- "Graduate in as little as 1 Year" -->
              <div class="col-benefits">

                <!-- Icon -->
                <div>
                  <i class="fa-solid fa-calendar-check"></i>
                </div>

                <!-- Title -->
                <h4>
                  Graduate in as little as 1 Year
                </h4>

                <!-- Text -->
                <div class="text-benefits">
                  Online post-graduate certificates are a popular way to develop your professional qualifications of Masterstudy.
                </div>
              </div>
            </div>
        </div>
      </section>

      <!-- "Course List" Section -->
      <section>
        <div class="container-sm">

          <!-- First Row -->
          <div class="row">

            <!-- Software Development -->
            <div class="software-dev">

              <!-- Course Image -->
              <img src="../assets/img/cat_1-1540x750.jpg" alt="software-devlopment_img">

              <!-- Course Description -->
              <div class="courses-description">

                <!-- Course Type -->
                <div>
                  Software Development
                </div>

                <!-- Total Courses -->
                <div>
                  5 Courses
                </div>
              </div>
            </div>

            <div class="col-wrapper">

              <!-- Art -->
              <div class="col-thin">

                <!-- Course Image -->
                <img src="../assets/img/cat_2-370x155.jpg" alt="art_img">

                <!-- Course Description -->
                <div class="courses-description">

                  <!-- Course Type -->
                  <div>
                    Art
                  </div>

                  <!-- Total Courses -->
                  <div>
                    8 Courses
                  </div>
                </div>
              </div>

              <!-- Material Design -->
              <div class="col-thin">

                <!-- Course Image -->
                <img src="../assets/img/cat_3-370x155.jpg" alt="material-design_img">

                <!-- Course Description -->
                <div class="courses-description">

                  <!-- Course Type -->
                  <div>
                    Material Design
                  </div>

                  <!-- Total Courses -->
                  <div>
                    5 Courses
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Second Row -->
          <div class="row">

            <!-- Music -->
            <div class="col-thin-bottom">

              <!-- Course Image -->
              <img src="../assets/img/cat_5-370x155.jpg" alt="music_img">

              <!-- Course Description -->
              <div class="courses-description">

                <!-- Course Type -->
                <div>
                  Music
                </div>

                <!-- Total Courses -->
                <div>
                  5 Courses
                </div>
              </div>
            </div>

            <!-- Exercise -->
            <div class="col-thin-bottom">

              <!-- Course Image -->
              <img src="../assets/img/cat_4-370x155.jpg" alt="exercise_img">

              <!-- Course Description -->
              <div class="courses-description">

                <!-- Course Type -->
                <div>
                  Exercise
                </div>

                <!-- Total Courses -->
                <div>
                  7 Courses
                </div>
              </div>
            </div>

            <!-- Photography -->
            <div class="col-thin-bottom">

              <!-- Course Image -->
              <img src="../assets/img/cat_6-370x155.jpg" alt="photography_img">

              <!-- Course Description -->
              <div class="courses-description">

                <!-- Course Type -->
                <div>
                  Photography
                </div>

                <!-- Total Courses -->
                <div>
                  4 Courses
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- "Limitess Learning" Section -->
      <section>
        <div class="colums-wrapper">

          <!-- Column Left -->
          <div class="col-left background-img">
            <div class="container-sm">

              <!-- Title -->
              <h2>
                Limitless learning, <br>
                more possibilities
              </h2>

              <!-- Subtitle -->
              <h3>
                Online course open the opportunity for learning to <br>
                almost anyone, regardless of their scheduling <br>
                commitments.
              </h3>

              <!-- Sign Up Button -->
              <a href="#" class="btn">
                  read more
              </a>
            </div>
          </div>
        </div>
      </section>
    </main>
</template>

<script>
export default {
name: "MainComponent",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

main {

  // "Start Investing" Section
  .colums-wrapper {
    display: flex;
    padding-top: 2rem;

    .col-left {
      width: 60%;
      padding-top: 7rem;
      padding-right: 1.8rem;
      padding-inline: 0.6rem;

      // Reuse for "Limitess Learning" Section
      &.background-img {
        width: 100%;
        background-image: url("../assets/img/Untitled-1-1-1-1-1.png");
        background-position: center;
        padding-bottom: 7rem;
      }

      h2 {
        font-size: 2.8rem;
        font-weight: 200;
      }

      h3 {
        font-size: 1rem;
        font-weight: 300;
        padding-block: 2rem;
      }

      .btn {
        font-weight: 600;
      }

      a {
        font-size: 0.7rem;
        display: inline-block;
        background-color:$color_cube6;
        color: $color_cube1;
        border: 1px solid $color_cube6;
        text-transform: uppercase;
        padding: 1rem 1.4rem;
        border-radius: 30px;
        cursor: pointer;
      }
    }

    .col-right {
      width: 40%;
      position: relative;
      
      .bg-img {
        width: 30rem;
      }

      .book1-img {
        width: 9rem;
        position: absolute;
        top: 90px;
        right: -97px;
      }

      .moon-img {
        width: 3.5rem;
        filter: grayscale(80%);
        position: absolute;
        top: 92px;
        right: 204px;
      }

      .bubblespeech-img {
        width: 3.5rem;
        position: absolute;
        top: 52px;
        right: -95px;
      }

      .book2-img {
        width: 11.5rem;
        position: absolute;
        bottom: 44px;
        right: -15px;
      }

      .magnifier-img {
        width: 3.8rem;
        position: absolute;
        bottom: 95px;
        right: -84px;
      }
    }
  }

  .benefits {
    display: flex;
    justify-content: space-between;
    padding-block: 4rem;

    .col-benefits {
      width: calc((100% / 3) - 1.5rem);
      background-color:$material_design6;
      margin: 0.6rem;
      padding: 1.6rem;

      i {
        font-size: 2rem;
        color: $color_cube6;
      }

      h4 {
        font-weight:400;
        font-size: 0.8rem;
        padding-block: 1.5rem;
      }

      .text-benefits {
        font-size: 0.6rem;
        color:$median_cut6;
      }
    }
  }
  
  // "Course List" Section
  .row {
    display: flex;
    justify-content: space-between;
    margin: 0.6rem;
  }

  .software-dev {
    width: calc(((100% / 3) - 0.25rem) * 2);
  }

  .courses-description {
    display: flex;
    justify-content: space-between;
    font-size: 0.7rem;
    padding-block: 1.16rem;
  }

  .col-wrapper {
    width: 34%;

    .col-thin {
      width: 100%;
      padding-left: 1.6rem;
    }
  }

  .col-thin-bottom {
    width: calc((100% / 3) - 1.2rem);
  }


}
</style>