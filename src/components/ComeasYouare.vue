<template>
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

                    <!-- Caret Right Icon (graphic element on right side div) -->
                    <div class="caret-right">
                        <i class="fa-solid fa-caret-right"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:"ComeasYouare"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

// "Come As You Are" Section
.comeasyouare {
    background-image: url(../assets/img/brooke-cagle-224821-unsplash-1-1920x700.jpg);
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: 90rem ;
    height: 32rem;
    position: relative;

.wrapper {
    background-color: $color_cube1;
    width: 40%;
    padding: 3.7rem;
    margin-left: 2.5rem;
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
</style>