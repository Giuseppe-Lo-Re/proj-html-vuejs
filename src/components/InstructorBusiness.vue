<template>
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
</template>

<script>
export default {
    name: "InstructorBusiness"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

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

</style>