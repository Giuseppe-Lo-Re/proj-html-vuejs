<template>
    <main>

      <!-- "Start Investing" Section -->
      <StartInvesting />
      
      <!-- "Course List" Section -->
      <CourseList />

      <!-- "Limitess Learning" Section -->
      <LimitessLearning />

      <!-- "Recent Course" Section -->
      <RecentCourse />

      <!-- "We are Proud" Section -->
      <WeareProud />

      <!-- Newsletter Section -->
      <NewsLetter />

      <!-- "Popular Course" Section -->
      <PopularCourse />

      <!-- "Instructor/Business" Section -->
      <section>
        <div class="container-lg">
          <div class="instructor-business">

            <!-- "Become an Instructor" -->
            <div class="col-left">
              
              <!-- Image -->
              <div class="img-container">
                <img src="../assets/img/image_box_1-221x231.png" alt="instructor">
              </div>

              <div class="wrapper">

                <!-- Title -->
                <h3>
                  Become an Instructor
                </h3>

                <!-- Subtitle -->
                <h4>
                  Teach what you love. Masterstudy gives you <br>
                  the tools to create a course.
                </h4>

                <!-- "Start Teaching" Button -->
                <a href="#" class="btn">
                    start teaching
                </a>
              </div>
            </div>

            <!-- "Setup For Business" -->
            <div class="col-right">
              
              <!-- Image -->
              <div class="img-container">
                <img src="../assets/img/image_box_2-234x231.png" alt="business">
              </div>

              <div class="wrapper">

                <!-- Title -->
                <h3>
                  Setup For Business
                </h3>

                <!-- Subtitle -->
                <h4>
                  Get Ulimited accesss to 2,500 of Udemy's top <br>
                  courses for your team.
                </h4>

                <!-- "Doing Business" Button -->
                <a href="#" class="btn">
                    doing business
                </a>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- "Come As You Are" Section -->
      <section>
        <div class="comeasyouare">
          <div class="container-sm">
            <div class="wrapper">

              <!-- Title -->
              <h3>
                Come as you are
              </h3>

              <!-- Text -->
              <p class="text">
                MasterStudy used is an excellent workshop whether you come <br>
                as a counselor, advisor, administrator, or faculty member. I am <br>
                going home empowered. I am looking forward to attending <br>
                the On Course MasterStudy and the MAsterStudy National <br>
                COnference next year and facilitating the use of this excellent <br>
                retention/student success course at my college.
              </p>

              <!-- Sign -->
              <div class="sign">
                Tim Sab
              </div>

              <!-- Role -->
              <div class="role">
                General Developer, Stylemix Themes
              </div>

              <!-- Caret Right Icon -->
              <div class="caret-right">
                <i class="fa-solid fa-caret-right"></i>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
</template>

<script>
import StartInvesting from "../components/StartInvesting";
import CourseList from "../components/CourseList";
import LimitessLearning from "../components/LimitessLearning";
import RecentCourse from "../components/RecentCourse";
import WeareProud from "../components/WeareProud";
import NewsLetter from "../components/NewsLetter";
import PopularCourse from "../components/PopularCourse";

export default {
  name: "MainComponent",
  components: {
    StartInvesting,
    CourseList,
    LimitessLearning,
    RecentCourse,
    WeareProud,
    NewsLetter,
    PopularCourse,

  }

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

        // Hover Effect
        &:hover {
          background-color: $color_cube8;
          border: none;
          transform: scale(1.1);
        }
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

      // Hover Effect
      &:hover {
        transform: scale(1.15);
        box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.5);
      }

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
    cursor: pointer;
  }

  .courses-description {
    display: flex;
    justify-content: space-between;
    font-size: 0.7rem;
    padding-block: 1.16rem;
    cursor: pointer;
  }

  .col-wrapper {
    width: 34%;

    .col-thin {
      width: 100%;
      padding-left: 1.6rem;
      cursor: pointer;
    }
  }

  .col-thin-bottom {
    width: calc((100% / 3) - 1.2rem);
    cursor: pointer;
  }

  // "Recent Course" Section
  .recent-course {
    text-align: center;
    position: relative;

    h2 {
      font-size: 2.5rem;
      font-weight: 200;
      padding-top: 3.5rem;
      padding-bottom: 1.5rem;
    }

    ul {
      display: flex;
      justify-content: center;
      align-items: center;
      
      li {
        list-style-type: none;
        font-size: 0.7rem;
        padding-inline: 1rem;
        font-weight: 300;
        color: $color_cube6;
        margin-bottom: 2rem;
        cursor: pointer;
      }

      .active {
        background-color:$material_design6;
        padding: 0.5rem 0.7rem;
        border-radius: 30px;
        color:$median_cut6;
      }
    }

    // Cards
    .cards-container {
      width: 90%;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      padding-bottom: 4rem;

      .card-container {
        width: calc(100% / 6);
        padding: 0.5rem;
        cursor: pointer;

        .card {
          border: 1px solid $median_cut2;
          position: relative;
          overflow: hidden;

          .sticker {
            color: $color_cube1;
            text-transform: uppercase;
            font-size: 0.6rem;
            padding: 0.1rem 0.25rem;
            border-radius: 3px;
            position: absolute;
            top: 10px;
            right: 10px;

            // Use for Rotated Sticker
            &.rotate-style {
              width: 7.8rem;
              height: 1.4rem;
              font-size: 0.5rem;
              font-weight: 800;
              padding-top: 0.4rem;
              transform: rotate(-45deg);
              position: absolute;
              top: 21px;
              right: 104px;
            }

            // Reuse with differents colors
            &.green {
              background-color: $color_cube2;
            }
            
            &.red {
              background-color: $color_cube8;
            }

            &.orange {
              background-color: $median_cut7;
            }
          }

          // Change color on selection
          &.selected {
          border: 1px solid $color_cube7;
          }

          // Hover effect
          &:hover {
            border: 1px solid $color_cube2;
            transform: scale(1.05);
            box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.5);
          }
          
          .details {
            padding: 0.9rem;

            .category {
              font-size: 0.6rem;
              color: $median_cut6;
              text-align: left;

              i {
                font-size: 0.5rem;
              }
            }

            .name {
              font-size: 0.7rem;
              text-align: left;
              padding-block: 0.8rem;
            }

            .card-footer {
              display: flex;
              justify-content: space-between;
              align-items: center;
              border-top: 1px solid $median_cut2;
              padding-top: 0.8rem;
              height: 2rem;

              .length {
                display: flex;
                align-content: center;
                color: $median_cut6;

                i {
                  font-size: 0.8rem;
                }

                .stars {

                  i {
                    font-size: 0.5rem;
                    color: $color_cube7;
                  }
                }

                .text {
                  font-size: 0.7rem;
                  padding-left: 0.2rem;

                  &.center {
                    padding-top: 0.35rem;
                  }
                }
              }

              .old-price {
                font-size: 0.60rem;
                font-weight: 500;
                text-decoration: line-through;
                color: $median_cut6;
              }

              .price,
              .new-price {
                font-size: 0.75rem;
                font-weight: 500;
              }
            }
          }
        }
      }

      .selected {
        border: 1px solid $color_cube7;
      }
    }

    .btn {
      font-weight: 600;
      margin-bottom: 4rem;
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

        // Hover Effect
        &:hover {
          background-color: $color_cube2;
          border: none;
          transform: scale(1.1);
        }
      }
  
  .utility-wrapper {
    box-shadow: 1.5px 5px 5px 1.5px rgba(0, 0, 0, 0.2);
    display: inline-block;
    padding: 0.8rem;
    margin-bottom: 0.5rem;
    position: absolute;
    bottom: 0;
    right: 0;

    .icon {
      padding-block: 0.6rem;
      color: $median_cut6;
      cursor: pointer;

      // Hover Effect
      &:hover {
        color: $color_cube2;
      }
    }
  }
}

  // "We are Proud" Section
  .we-are-proud {
    background-color: $material_design6;
    background-image: url("../assets/img/we_proud.png");
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: 1500px;
    padding-top: 4rem;
    padding-bottom:18rem;
    text-align: center;

    .titles-wrapper {
        width: 50%;
        margin: 0 auto;

      h2 {
        font-size: 2.5rem;
        font-weight: 200;
      }
  
      h3 {
        font-size: 1rem;
        font-weight: 300;
        padding-block: 2rem;
      }
    }

    .numbers {
      width: 80%;
      margin: 0 auto;
      display: flex;
      justify-content: space-evenly;

      .numbers-wrapper {
        padding-inline: 5rem;
        border-right: 2px solid $median_cut2;

        &.no-border {
          border-right: none;
        }

        .number {
          font-size: 3rem;
          font-weight: 300;
          padding-bottom: 0.7rem;
        }

        .text {
          font-size: 0.9rem;
          font-weight: 100;
          text-transform: uppercase;
        }
      }
    }
  }

  // Newletter Section
  .newletter {
    color: $color_cube1;
    background-color: $color_cube2;

    .cols-wrapper {
      display: flex;
      padding-block: 3rem;

      h4 {
          font-size: 0.8rem;
          font-weight: 500;
          padding-bottom: 0.6rem;
        }

      .col-left {
        width: 60%;

        p {
          font-size: 0.7rem;
          font-weight: 300;
        }
      }

      .col-right {
        width: 40%;
        padding-left: 1rem;

        h4 {
          text-transform: uppercase;
          font-size: 00.7rem;
          font-weight: 400;
        }
      }

      .form {
        display: flex;

        input {
          display: inline;
          font-size: 0.75rem;
          padding: 0.5rem;
          width: 21.5rem;
          background-color: $material_design6;
          border: none;
      }

        textarea:focus, input:focus {
          outline: none;
        }

        button {
          background-color: $color_cube6;
          border: none;
          padding: 0.7rem 0.8rem;
          text-transform: uppercase;
          color: $color_cube1;
          font-size: 0.7rem;
          cursor: pointer;
        }
      }
    }
  }

  // "Popular Courses" Section
  .popular-courses {
    text-align: center;
    position: relative;
    background-color: $material_design6;

    h2 {
      font-size: 2.5rem;
      font-weight: 200;
      padding-top: 3.5rem;
      padding-bottom: 1.5rem;
    }

    ul {
      display: flex;
      justify-content: center;
      align-items: center;
      
      li {
        list-style-type: none;
        font-size: 0.7rem;
        padding-inline: 1rem;
        font-weight: 300;
        color: $color_cube6;
        margin-bottom: 2rem;
        cursor: pointer;
      }

      .active {
        background-color:$material_design6;
        padding: 0.5rem 0.7rem;
        border-radius: 30px;
        color:$median_cut6;
      }
    }

    // Cards
    .cards-container {
      width: 90%;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      padding-bottom: 3rem;

      .card-container {
        width: calc(100% / 6);
        padding: 0.5rem;
        cursor: pointer;

        .card {
          border: 1px solid $median_cut2;
          position: relative;
          overflow: hidden;

          .sticker {
            color: $color_cube1;
            text-transform: uppercase;
            font-size: 0.6rem;
            padding: 0.1rem 0.25rem;
            border-radius: 3px;
            position: absolute;
            top: 10px;
            right: 10px;

            // Use for Rotated Sticker
            &.rotate-style {
              width: 7.8rem;
              height: 1.4rem;
              font-size: 0.5rem;
              font-weight: 800;
              padding-top: 0.4rem;
              transform: rotate(-45deg);
              position: absolute;
              top: 21px;
              right: 104px;
            }

            // Reuse with differents colors
            &.green {
              background-color: $color_cube2;
            }
            
            &.red {
              background-color: $color_cube8;
            }

            &.orange {
              background-color: $median_cut7;
            }
          }

          // Change color on selection
          &.selected {
          border: 1px solid $color_cube7;
          }
          
          // Hover effect
          &:hover {
            border: 1px solid $color_cube2;
            transform: scale(1.05);
            box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.5);
          }

          .details {
            padding: 0.9rem;
            background-color: $color-cube1;

            .category {
              font-size: 0.6rem;
              color: $median_cut6;
              text-align: left;

              i {
                font-size: 0.5rem;
              }
            }

            .name {
              font-size: 0.7rem;
              text-align: left;
              padding-block: 0.8rem;
            }

            .card-footer {
              display: flex;
              justify-content: space-between;
              align-items: center;
              border-top: 1px solid $median_cut2;
              padding-top: 0.8rem;
              height: 2rem;

              .length {
                display: flex;
                align-content: center;
                color: $median_cut6;

                i {
                  font-size: 0.8rem;
                }

                .stars {

                  i {
                    font-size: 0.5rem;
                    color: $color_cube7;
                  }
                }

                .text {
                  font-size: 0.7rem;
                  padding-left: 0.2rem;

                  &.center {
                    padding-top: 0.35rem;
                  }
                }
              }

              .old-price {
                font-size: 0.60rem;
                font-weight: 500;
                text-decoration: line-through;
                color: $median_cut6;
              }

              .price,
              .new-price {
                font-size: 0.75rem;
                font-weight: 500;
              }
            }
          }
        }
      }

      .selected {
        border: 1px solid $color_cube7;
      }
    }
  }

  // "Turn Page" Button
  .turn-page {
    display: flex;
    justify-content: center;
    padding-bottom: 4rem;

    div {
      background-color: $color_cube1;
      border: 1px solid $median_cut2;

      i {
        font-size:0.7rem;
        padding: 0.7rem 0.8rem;
        color: $median_cut2;
        cursor: pointer;

        // Hover Effect
        &:hover {
          border: none;
          background-color: $median_cut1;
        }

      }
    }
  }

  // "Instructor/Business" Section
  .instructor-business {
    display: flex;
    padding-block: 4.5rem;

    .img-container {
      padding-left: 2rem;

      img {
      width: 10.5rem;
      }
    }

    h3 {
      font-size: 1.65rem;
      font-weight: 300;
    }

    h4 {
      font-size: 0.8rem;
      font-weight: 200;
      padding-top: 1.2rem;
    }

    .wrapper {
      padding-top: 1rem;
      padding-left: 3rem;
    }

    .col-left,
    .col-right {
      width:50%;
      display: flex;
      border: 1px solid $median_cut2;
      padding-top: 3rem;
      margin: 0.7rem;
    }

    .btn {
        font-weight: 600;
        margin-top: 1.5rem;
        margin-bottom: 4rem;
      }

      a {
        font-size: 0.7rem;
        display: inline-block;
        background-color:$color_cube6;
        color: $color_cube1;
        border: 1px solid $color_cube6;
        text-transform: uppercase;
        padding: 0.8rem 1.3rem;
        border-radius: 30px;
        cursor: pointer;

        // Hover Effect
        &:hover {
          background-color: $color_cube2;
          border: none;
          transform: scale(1.1);
        }
      }
  }

  // "Come As You Are" Section
  .comeasyouare {
    background-image: url(../assets/img/brooke-cagle-224821-unsplash-1-1920x700.jpg);
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: 90rem ;
    height: 33rem;
    position: relative;

    .wrapper {
      background-color: $color_cube1;
      width: 40%;
      padding: 3.5rem;
      margin-left: 2rem;
      position: absolute;
      top: 72px;
      left: 255px;

      h3 {
        font-size: 1.65rem;
        font-weight: 300;
      }

      p {
        font-size: 0.9rem;
        font-weight: 200;
        padding-block: 1.5rem;
        line-height: 1.4rem;
        position: relative;
      }

      .sign {
        font-size: 0.9rem;
        font-weight: 500;
      }

      .role {
        font-size: 0.7rem;
        font-weight: 300;
        padding-top: 0.2rem;
        padding-bottom: 1.6rem;
      }

      .caret-right {
        font-size: 4rem;
        color: $color-cube1;
        position: absolute;
        top: 146px;
        right: -17px;
      }
    }
  }
}
</style>