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

                        <!-- V-for links via props from data "headerLinks" -->
                        <li 
                            v-for="(link, index) in links"
                            :key= "index"
                        >
                            <!-- Notification -->
                            <div 
                                v-if="link.isNew"  
                                :class="{'new':link.isNew, 'on-second':link.isNew, }">
                                new
                            </div>

                            <a :href="link.url">
                                {{ link.category }}
                            </a>
                        </li>
                    </ul>

                    <!-- Socials Links -->
                    <ul class="socials-links">

                        <!-- V-for icons via props from data "socialsLinks" -->
                        <li 
                            v-for="(social, index) in socials"
                            :key="index"
                        >
                            <a :href="social.url"></a>
                            <i :class="social.icon"></i>
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
                    <input type="text" placeholder="Search courses">

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

                        <!-- Bookmark Icon -->
                        <div class="bookmark">
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
name: "HeaderComponent",
props: { 
    links: Array,
    socials: Array
}
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

                li {
                    list-style-type: none;
                    padding-inline: 0.55rem;
                    position: relative;
                    cursor: pointer;

                    .new {
                        background-color: $color_cube8;
                        color: $color_cube1;
                        text-transform: uppercase;
                        font-size: 0.45rem;
                        padding: 0.05rem 0.25rem;
                        margin-top: 0.2rem;
                        border-radius: 3px;
                        border-bottom-left-radius: 0px;

                        &.on-second {
                            position: absolute;
                            top: -18px;
                            left: 32px;
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
                padding-left: 1.5rem;
                display: flex;
                font-size: 0.75rem;
                
                li {
                    list-style-type: none;
                    padding-inline: 0.3rem;
                    cursor: pointer;
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
            width: 14rem;
            padding-right: 2rem;
            cursor: pointer;
        }

        .category {
            text-transform: uppercase;
            font-weight: 600;
            font-size: 0.6rem;
            padding-right: 0.6rem;
            cursor: pointer;
        }

        .form {

            input {
                display: inline;
                font-size: 0.7rem;
                padding: 0.8rem;
                width: 21.5rem;
                background-color: $material_design6;
                border: none;
            }

            ::placeholder {
                color: $median_cut6;
                opacity: 1; 
                }

            textarea:focus, input:focus {
                outline: none;
            }

            button {
                background-color: $color_cube6;
                border: none;
                padding: 0.65rem 0.55rem;
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
            padding-left: 2.3rem;
            font-size: 0.65rem;

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
                padding-left: 1.2rem;
                padding-right: 3.5rem;
            }

            .log-in {
                color: $color_cube6;
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
                    text-transform: uppercase;
                    padding: 0.6rem 1.2rem;
                    border-radius: 20px;
                    transition: all 1000ms;

                    // Hover Effect
                    &:hover {
                        background-color: $color_cube8;
                        border: none;
                        transform: scale(1.1);
                    }
                }

                .bookmark {
                    padding-right: 0.3rem;
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