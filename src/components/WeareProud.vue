<template>

    <!-- "We are Proud" Section -->
    <section>
        <div class="we-are-proud">
            <div class="titles-wrapper">

                <!-- Title -->
                <h2>
                    We are Proud
                </h2>

                <!-- Subtitle -->
                <h3>
                    Certificate courses are instructed by hightly educated and qualified instructors who hold doctoral and master's level degrees.
                </h3>
            </div>

            <!-- Numbers -->
            <div class="numbers">

                <!-- Students -->
                <div class="numbers-wrapper">

                    <!-- Number -->
                    <div class="number">
                        2000
                    </div>

                    <!-- Text -->
                    <div class="text">
                        students
                    </div>
                </div>

                <!-- Courses -->
                <div class="numbers-wrapper">

                    <!-- Number -->
                    <div class="number">
                        950
                    </div>

                    <!-- Text -->
                    <div class="text">
                        courses
                    </div>
                </div>

                <!-- Hours Video -->
                <div class="numbers-wrapper">

                    <!-- Number -->
                    <div class="number">
                        1600
                    </div>

                    <!-- Text -->
                    <div class="text">
                        hours video
                    </div>
                </div>

                <!-- Countries Reached -->
                <div class="numbers-wrapper no-border">

                    <!-- Number -->
                    <div class="number">
                        150
                    </div>

                    <!-- Text -->
                    <div class="text">
                        country reached
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "WeareProud"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

// "We are Proud" Section
.we-are-proud {
    background-color: $material_design6;
    background-image: url("../assets/img/we_proud.png");
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: 1500px;
    padding-top: 4rem;
    padding-bottom: 15rem;
    text-align: center;

    .titles-wrapper {
        width: 44%;
        margin: 0 auto;

        h2 {
            font-size: 2.3rem;
            font-weight: 200;
        }

        h3 {
            font-size: 0.9rem;
            font-weight: 100;
            padding-block: 2rem;
        }
    }

    .numbers {
        width: 80%;
        margin: 0 auto;
        padding-top: 3rem;
        display: flex;
        justify-content: space-evenly;

        .numbers-wrapper {
            padding: 2rem 5rem;
            border-right: 1px solid $median_cut2;

            &.no-border {
                border-right: none;
            }

            .number {
                font-size: 3rem;
                font-weight: 200;
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
</style>