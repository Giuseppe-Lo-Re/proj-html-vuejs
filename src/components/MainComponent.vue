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

  .colums-wrapper {
    display: flex;
    padding-top: 2rem;

    .col-left {
      width: 60%;
      padding-top: 7rem;
      padding-right: 1.8rem;

      h2 {
        font-size: 2.8rem;
        font-weight: 100;
      }

      h3 {
        font-size: 1rem;
        font-weight: 100;
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
        top: 94px;
        right: -97px;
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
}
</style>