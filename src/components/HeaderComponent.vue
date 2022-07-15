<template>
    <header>
        <!-- Header Top -->
        <div class="container-lg">
            <div class="header-top">

                <!-- Language Menù-->
                <div class="language-menu">

                    <!-- Language text -->
                    <div class="language-text">
                        English
                    </div>

                    <!-- Chevron-down Icon -->
                    <span class="chevron-down">
                        <i class="fa-solid fa-chevron-down fa-xs"></i>
                    </span>
                </div>
                
                <!-- Navbar Top-->
                <div class="navbar-top">
                    <!-- Menu Links -->
                    <ul class="menu-links">

                        <li>
                            link
                        </li>

                        <li class="relative">
                            <!-- Notification -->
                            <div class="new on-second">
                                new
                            </div>
                            link
                        </li>

                        <li>
                            link
                        </li>

                        <li>
                            link
                        </li>

                        <li>
                            link
                        </li>

                        <li>
                            <!-- Notification -->
                            <div class="new on-sixth">
                                new
                            </div>

                            link
                        </li>

                        <li>
                            link
                        </li>
                    </ul>

                    <!-- Socials Links -->
                    <ul class="socials-links">

                        <li>
                            <i class="fa-brands fa-twitter"></i>
                        </li>

                        <li>
                            <i class="fa-brands fa-instagram"></i>
                        </li>

                        <li>
                            <i class="fa-brands fa-behance"></i>
                        </li>

                        <li>
                            <i class="fa-solid fa-basketball"></i>
                        </li>

                        <li>
                            <i class="fa-solid fa-wand-magic-sparkles"></i>
                        </li>

                        <li>
                            <i class="fa-brands fa-git"></i>
                        </li>

                        <li>
                            <i class="fa-brands fa-linkedin"></i>
                        </li>

                        <li>
                            <i class="fa-brands fa-pinterest"></i>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
    </header>
</template>

<script>
export default {
name: "HeaderComponent"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

header {
    padding: 1.25rem;
    .header-top {
        display: flex;
        justify-content: space-between;
        border-bottom: 0.063rem solid lightgrey;
        color:grey;
        font-size: 0.625rem;
        padding-bottom: 0.625rem;
    
        .language-menu {
            display: flex;
            cursor: pointer;
    
            .chevron-down {
                padding-left: 0.313rem;
            }
        }

        .navbar-top {
            display: flex;

            .menu-links {
                display: flex;
                position: relative;
        
                li {
                    list-style-type: none;
                    padding-inline: 0.6rem;
                    cursor: pointer;

                    .new {
                        background-color: $color_cube8;
                        color: $color_cube1;
                        padding: 0.1rem 0.25rem;
                        border-radius: 5px;
                        border-bottom-left-radius: 0px;

                    &.on-second {
                        position: absolute;
                        top: -18px;
                        left: 54px;
                    }

                    &.on-sixth {
                        position: absolute;
                        top: -18px;
                        right: 33px;
                    }
                    }

                }
            }
    
            .socials-links {
                padding-left: 1.875rem;
                display: flex;
        
                li {
                    list-style-type: none;
                    padding-inline: 0.3rem;
                    cursor: pointer;
                }
            }

        }
    }
    
}
</style>