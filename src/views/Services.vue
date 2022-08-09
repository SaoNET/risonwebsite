<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100">
            <h1 class="title">Web Development Services</h1>
            <!-- <h4>
              Every landing page needs a small description after the big bold
              title, that's why we added this text here. Add here all the
              information that can make you or your product create the first
              impression
            </h4> -->
            <!-- <br />
            <md-button
              href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
              class="md-success md-lg"
              target="_blank"
              ><i class="fas fa-play"></i> Watch video</md-button
            > -->
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section">
        <div class="container">
          <div class="md-layout md-gutter">
            <div class="md-layout-item md-small-size-100" style="margin: 10% 0;">
              <h3>Web Aplant is a leading web development company 
                delivering complex web projects way beyond regular website building</h3>
            </div>
            <div class="md-layout-item md-medium-size-40 md-small-size-100" style="background-color: whitesmoke;">
              <div>
                <h4 class="title">EXTENSIVE EXPERIENCE</h4>
                <h5 class="description">
                  For over a decade, we have developed thousands of outstanding projects 
                  that have helped our customers accomplish their business goals
                </h5>
              </div>
              <div>
                <h4 class="title">INDUSTRY-FOCUSED SPECIALISTS</h4>
                <h5 class="description">
                  With a strong focus on technology-intensive industries and constant attention 
                  to detail and IT trends, Web Aplant's specialists help companies from all over the world
                </h5>
              </div>
              <div>
                <h4 class="title">CUSTOMER LOYALTY</h4>
                <h5 class="description">
                  Web Aplant’s high standards, effective project delivery, 
                  and ability to develop IT solutions of any kind 
                  enable us to enjoy wide recognition. As a result, 
                  90% of our customers are recurring and recommend us to their business partners
                </h5>
              </div>
            </div>
            <div class="md-layout-item md-medium-size-20 md-small-hide md-alignment-center-center" style="background-color: whitesmoke;">
              <div style="height: 30%;">
                <h3>
                  10+
                </h3>
                <h5>successful projects</h5>
              </div>
              <div style="height: 30%;">
                <h3>
                  5
                </h3>
                <h5>years in business</h5>
              </div>
              <div style="height: 30%;">
                <h3>
                  90%
                </h3>
                <h5>recurring customers</h5>
              </div>
            </div>
          </div>
          <div class="md-layout md-gutter md-alignment-center-space-around" style="background-color: currentcolor; padding: 5% 0;">
            <div class="md-layout-item md-small-size-50">
              <img src="../assets/img/logos/microsoft.svg"/>
              <p class="title" style="color: white;">Microsoft certified</p>
            </div>
            <div class="md-layout-item md-small-size-50">
              <img src="../assets/img/logos/clutch-90-reviews.svg"/>
              <p class="title" style="color: white;">High ratings</p>
            </div>
            <div class="md-layout-item md-small-size-50">
              <img src="../assets/img/logos/b2b-2020.svg"/>
              <p class="title" style="color: white;">B2B company</p>
            </div>
            <div class="md-layout-item md-small-size-50">
              <img src="../assets/img/logos/aws-white.svg"/>
              <p class="title" style="color: white;">AWS Partner</p>
            </div>
          </div>
          <div class="md-layout md-gutter">
            <div class="md-layout-item md-small-size-100">
              <h2 class="title">Websites</h2>
              <h5 class="description">
                Webaplant builds feature-rich and reliable websites, with advanced UI/UX and intuitive user flows, 
                for businesses and non-profit organizations, so that you can raise visibility, win new audiences, 
                and communicate your advantages
              </h5>
            </div>
            <div class="md-layout-item md-small-size-100">
              <h2 class="title">Web portals</h2>
              <h5 class="description">
                A webportal built by Webaplant’s tech experts for your organization will be fully capable of collecting 
                all the data you need from different sources and presenting that data in a uniform and convenient way
              </h5>
            </div>
            <div class="md-layout-item md-small-size-100">
              <h2 class="title">Ecommerce</h2>
              <h5 class="description">
                Whatever your business model is — be it a marketplace or B2C and B2B projects — Webaplant’s web developers 
                will take care of each relevant eCommerce component and seamlessly integrate it into a web app
              </h5>
            </div>
            <div class="md-layout-item md-small-size-100">
              <h2 class="title">Enterprise web solutions</h2>
              <h5 class="description">
                Building enterprise-grade web solutions for huge amounts of data with Webaplant will provide your business 
                with advanced capabilities for knowledge sharing, monitoring, management, and decision-making
              </h5>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  bodyClass: "landing-page",
  props: {
    header: {
      type: String,
      default: require("@/assets/img/headers/eminent-spirit.gif")
    },
    teamImg1: {
      type: String,
      default: require("@/assets/img/faces/avatar.jpg")
    },
    teamImg2: {
      type: String,
      default: require("@/assets/img/faces/christian.jpg")
    },
    teamImg3: {
      type: String,
      default: require("@/assets/img/faces/kendall.jpg")
    }
  },
  data() {
    return {
      name: null,
      email: null,
      message: null
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  }
};
</script>

<style lang="scss" scoped>
.md-card-actions.text-center {
  display: flex;
  justify-content: center !important;
}
.contact-form {
  margin-top: 30px;
}

.md-has-textarea + .md-layout {
  margin-top: 15px;
}
</style>
