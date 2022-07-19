<template>

  <!-- "Categories Courses" Section -->
    <section>
        <div class="container-sm">

            <!-- First Row -->
            <div class="row">

                <!-- Software Development -->
                <div class="software-dev">

                    <!-- Category Image -->
                    <img src="../assets/img/cat_1-1540x750.jpg" alt="software-devlopment">

                    <!-- Course Details -->
                    <div class="courses-details">

                        <!-- Category Course -->
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

                        <!-- Category Image -->
                        <img src="../assets/img/cat_2-370x155.jpg" alt="art">

                        <!-- Course Details -->
                        <div class="courses-details">

                            <!-- Category Course -->
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

                        <!-- Category Image -->
                        <img src="../assets/img/cat_3-370x155.jpg" alt="material-design">

                        <!-- Course Details -->
                        <div class="courses-details">

                            <!-- Category Course -->
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

                    <!-- Category Image -->
                    <img src="../assets/img/cat_5-370x155.jpg" alt="music">

                    <!-- Course Details -->
                    <div class="courses-details">

                        <!-- Category Course -->
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

                    <!-- Category Image -->
                    <img src="../assets/img/cat_4-370x155.jpg" alt="exercise">

                    <!-- Course Details -->
                    <div class="courses-details">

                        <!-- Category Course -->
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
                    <img src="../assets/img/cat_6-370x155.jpg" alt="photography">

                    <!-- Category Details -->
                    <div class="courses-details">

                        <!-- Category Course -->
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
</template>

<script>
export default {
    name: "CategoriesCourses"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

// "Categories Courses" Section
.row {
    display: flex;
    justify-content: space-between;
    margin: 0.6rem;
}

.software-dev {
    width: calc(((100% / 3) - 0.25rem) * 2);
    cursor: pointer;
}

.courses-details {
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
</style>