<template>

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

            <!-- "Join for Free" Button -->
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
</template>

<script>
export default {
    name: "StartInvesting"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

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
</style>