<template>
  <footer>
    <div class="container-sm">
      <ul>

        <!-- About -->
        <li>

          <!-- Title -->
          <h5>
            About
          </h5>

          <!-- text -->
          <p class="text">

            <!-- Link -->
            <a href="/">
            Masterstudy
            </a>

            is Education Wordpress theme <br>
            featured by Learning Management System <br>
            (LMS) for online education. <br>
            Developed by

            <!-- Link -->
            <a href="/">
            StylemixThemes.
            </a>
          </p>

          <!-- Socials Links -->
          <ul class="socials-links">
            
            <li>
                <i class="fa-brands fa-facebook"></i>
            </li>

            <li>
                <i class="fa-brands fa-twitter"></i>
            </li>

            <li>
                <i class="fa-brands fa-instagram"></i>
            </li>
          </ul>
        </li>

        <!-- Contact -->
        <li>

          <!-- Title -->
          <h5>
            Contact
          </h5>

          <!-- Address -->
          <p class="text">
            USA, California 20, FIrst Avenue, <br>
            California
          </p>

          <div class="phone-numbers">

            <!-- Phone Number -->
            <div>
              Tel.: +1 212 458 300 32
            </div>

            <!-- Fax Number -->
            <div>
              Fax.: +1 212 375 24 14
            </div>
          </div>

          <div class="mail">
            info@masterstudy.com
          </div>
        </li>

        <!-- Page -->
        <li class="pages">

          <!-- Title -->
          <h5>
            Pages
          </h5>

          <div class="ul-wrapper">
            <ul>
              <li>
                <span>link</span> 
              </li>

              <li>
                <span>link</span> 
              </li>


              <li>
                <span>link</span> 
              </li>

            </ul>

            <ul>
              <li>
                <span>link</span> 
              </li>

              <li>
                <span>link</span> 
              </li>


              <li>
                <span>link</span> 
              </li>

            </ul>
          </div>
        </li>

        <!-- Blog -->
        <li>

          <!-- Title -->
          <h5>
            Blog
          </h5>

          <div class="news-wrapper">

            <!-- Image -->
            <img src="../assets/img/photo-1517520287167-4bbf64a00d66-50x50.jpeg" alt="news-blog-1">

            <div class="text-wrapper">

              <!-- Title -->
              <h5>
                Our main target is to <br>
                "Developing Yourself as <br>
                a Leader"
              </h5>

              <!-- Date -->
              <div class="date">

                <!-- Two-Em Dash Unicode -->
                <span class="dash">
                  &#11834;
                  </span> 
                  
                  August 9, 2018
              </div>
            </div>
          </div>

          <div class="news-wrapper">

            <!-- Image -->
            <img src="../assets/img/photo-1490376840453-5f616fbebe5b-50x50.jpeg" alt="news-blog-2">

            <div class="text-wrapper">

              <!-- Title -->
              <h5>
                Those Other College <br>
                Expenses You Aren't <br>
                Thinking About
              </h5>

              <!-- Date -->
              <div class="date">

                <!-- Two-Em Dash Unicode -->
                <span class="dash">
                  &#11834;
                  </span> 

                  June 3, 2015
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
name: "FooterComponent"
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

footer {
  padding-top: 2.7rem;
  padding-bottom: 1.5rem;

  ul {
    display: flex;

    li {
      list-style-type: none;
      padding-inline: 1rem;

      h5 {
        padding-bottom: 0.8rem;
      }

      p,
      div {
        font-size: 0.6rem;
        font-weight: 300;

        a {
          color: $color_cube6;
        }
      }

      .socials-links {
        display: flex;
        padding-top: 0.8rem; 

        i {
        color:$median_cut6;
        cursor: pointer;
      }
      }

      .phone-numbers {
        padding-block: 1rem;
      }

      .mail {
        color:$median_cut6;
        cursor: pointer;
      }
    }

    .pages {
      padding-left: 1rem;
      
      .ul-wrapper {
        display: flex;
        margin-left: 0.7rem;
      }

      ul {
        display: block;

        li {
          padding-right: 2rem;
          cursor: pointer;
        }
      }

      li {
        list-style-type: disc;
        font-size: 0.7rem;
        padding-block: 0.3rem;

        // Reduce space from bullet to li
        span {
          position: relative;
          left: -10px;
        }
      }
    }

    .news-wrapper {
      display: flex;
      padding-bottom: 1rem;
      cursor: pointer;

      img {
        width: 4rem;
        height: 4rem;
      }

      .text-wrapper {
        padding-left: 1rem;
        color: $median_cut6;

        h5 {
          font-size: 0.7rem;
        }

        .date {
          font-weight: 300;

          .dash {
            font-size: 0.4rem;
            padding-right: 0.1rem;
          }
        }
      }
    }
  }
}
</style>