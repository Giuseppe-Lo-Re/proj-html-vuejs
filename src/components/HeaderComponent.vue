<template>
    <header>

        <!-- Header Top -->
        <div class="header-top">
            <div class="container-lg flex">
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
                            <i class="fa-brands fa-flickr"></i>
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

        <!-- Header Bottom -->
        <div class="header-bottom">
            <div class="container-lg flex">

                <!-- Logo -->
                <div class="logo">
                    <img src="../assets/img/MasterStudy_logo.svg" alt="masterstudy_logo">
                </div>

                <!-- Category -->
                <div class="category">

                    <!-- Bars Icon -->
                    <i class="fa fa-bars" aria-hidden="true"></i>
                    category
                </div>

                <!-- Form -->
                <div class="form">

                    <!-- Input -->
                    <input type="text" placeholder="Search course">

                    <!-- Button -->
                    <button type="submit">
                        <i class="fa fa-search" aria-hidden="true"></i>
                    </button>
                </div>

                <!-- Call to Action -->
                <div class="cta">

                    <!-- Instructor -->
                    <div class="instructor">

                        <!-- Megaphone Icon -->
                        <i class="fa-solid fa-chalkboard-user"></i>
                        Become an Instructor
                    </div>

                    <!-- Enterprise -->
                    <div class="enterprise">

                        <!-- Instructor Icon -->
                        <i class="fa-solid fa-suitcase"></i>
                        For Enterprise
                    </div>

                    <!-- User Access -->
                    <div class="user-access">
                        <!-- Log in -->
                        <div class="log-in">

                            <!-- User Icon -->
                            <i class="fa-solid fa-user"></i>
                            log in
                        </div>

                        <!-- "Sign Up" Button -->
                        <a href="#" class="btn">
                            sign up
                        </a>

                        <div class="bookmark">

                            <!-- Bookmark Icon -->
                            <i class="fa-regular fa-bookmark fa-xl"></i>
                        </div>
                    </div>
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
    padding-block: 1.25rem;
    .header-top {
        border-bottom: 0.063rem solid lightgrey;
        color:$median_cut6;
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
                        text-transform: uppercase;
                        font-size: 0.5rem;
                        padding: 0.1rem 0.25rem;
                        border-radius: 3px;
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
                font-size: 0.75rem;
                
        
                li {
                    list-style-type: none;
                    padding-inline: 0.3rem;
                    cursor: pointer;

                    i {
                        // Hover Effect
                        &:hover {
                            color: $color_cube8;
                        }
                    }
                }
            }
        }
    }

    .header-bottom {
        display: flex;
        align-items: center;
        color: $median_cut6;
        padding-top: 1rem;

        .logo {
            width: 16rem;
            padding-right: 2rem;
            cursor: pointer;
        }

        .category {
            text-transform: uppercase;
            font-weight: 500;
            font-size: 0.6rem;
            // padding-right: 0.rem;
            cursor: pointer;
        }

        .form {
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
                padding: 0.43rem;
                cursor: pointer;

                i {
                    color: $color_cube1;
                    padding-inline: 0.5rem;
                }
            }
        }

        .cta {
            display: flex;
            align-items: center;
            padding-left: 2.5rem;
            font-size: 0.7rem;

            .instructor,
            .enterprise,
            .log-in {
                cursor: pointer;
            }

            i {
                color: $color_cube6;
                padding-inline: 0.2rem;
            }

            .enterprise {
                padding-inline: 1.2rem;
            }

            .user-access {
                display: flex;
                align-items: center;

                .btn {
                    font-weight: 600;
                    margin-inline: 1.3rem;
                }

                a {
                    display: inline-block;
                    background-color:$color_cube6;
                    color: $color_cube1;
                    border: 1px solid $color_cube6;
                    text-transform: uppercase;
                    padding: 0.6rem 1.2rem;
                    border-radius: 20px;
                    cursor: pointer;

                    // Hover Effect
                    &:hover {
                        background-color: $color_cube8;
                        border: none;
                        transform: scale(1.1);
                    }
                }

                .bookmark {
                    cursor: pointer;
                }
            }
        }
    }  
}
.flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>