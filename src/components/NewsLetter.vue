<template>

    <!-- Newsletter Section -->
    <section>
        <div class="newletter">
            <div class="container-sm">
                <div class="cols-wrapper">

                    <!-- Column Left -->
                    <div class="col-left">

                        <!-- Title -->
                        <h4>
                            Subscribe our newletter
                        </h4>

                        <!-- Subtitle -->
                        <p>
                            There are many cariations of passages of Lorem Ipsum avaiable, but the majority have <br>
                            suffered alteration in some form, by injected humour, or randomised words
                        </p>
                    </div>

                    <!-- Column Right -->
                    <div class="col-right">

                        <!-- Label -->
                        <h4>
                            Your e-mail address
                        </h4>

                        <!-- Form -->
                        <div class="form">

                            <!-- Input -->
                            <input type="text" placeholder="Enter you E-mail">

                            <!-- Button -->
                            <button type="submit">
                                subscribe
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "NewsLetter"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

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
                color: $median_cut6;
                font-size: 0.75rem;
                padding: 0.5rem;
                width: 21.5rem;
                background-color: $material_design6;
                border: none;
            }

            ::placeholder {
                color: $median_cut4;
                opacity: 1; 
            }

            textarea:focus, input:focus {
                outline: none;
            }

            button {
                background-color: $color_cube6;
                border: none;
                padding: 0.6rem 1rem;
                text-transform: uppercase;
                color: $color_cube1;
                font-size: 0.7rem;
                cursor: pointer;
            }
        }
    }
}
</style>