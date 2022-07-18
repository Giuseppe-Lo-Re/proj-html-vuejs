<template>

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

            <!-- "Read More" Button -->
            <a href="#" class="btn">
                read more
            </a>
        </div>
        </div>
    </div>
    </section>
</template>

<script>
export default {
  name: "LimitessLearning"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

// "Limitess Learning" Section
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
        text-transform: uppercase;
        padding: 1rem 1.4rem;
        border-radius: 30px;
        cursor: pointer;
        transition: all 1000ms;

        // Hover Effect
        &:hover {
          background-color: $color_cube7;
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

</style>