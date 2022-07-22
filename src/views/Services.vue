<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100">
            <h1 class="title">Your automation starts here.</h1>
            <h4>
              Every landing page needs a small description after the big bold
              title, that's why we added this text here. Add here all the
              information that can make you or your product create the first
              impression
            </h4>
            <br />
            <md-button
              href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
              class="md-success md-lg"
              target="_blank"
              ><i class="fas fa-play"></i> Watch video</md-button
            >
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section">
        <div class="container">
          <div class="md-layout md-gutter">
            <div class="md-layout-item">
              <h2 class="title">Let's talk product. Services</h2>
              <h5 class="description">
                This is the paragraph
              </h5>
            </div>
            <div class="md-layout-item md-size-50">
              <div>
                <h4 class="title">First</h4>
                <h5 class="description">
                  This is the paragraph
                </h5>
              </div>
              <div>
                <h4 class="title">Second</h4>
                <h5 class="description">
                  This is the paragraph
                </h5>
              </div>
              <div>
                <h4 class="title">Third</h4>
                <h5 class="description">
                  This is the paragraph
                </h5>
              </div>
            </div>
          </div>
          <div class="md-layout md-gutter">
            <div class="md-layout-item">
              <h3 class="title">Image 1</h3>
            </div>
            <div class="md-layout-item">
              <h3 class="title">Image 2</h3>
            </div>
            <div class="md-layout-item">
              <h3 class="title">Image 3</h3>
            </div>
            <div class="md-layout-item">
              <h3 class="title">Image 4</h3>
            </div>
          </div>
          <div class="md-layout md-gutter">
            <div class="md-layout-item md-size-50">
              <h2 class="title">Let's talk product</h2>
              <h5 class="description">
                This is the paragraph
              </h5>
            </div>
            <div class="md-layout-item md-size-50">
              <h2 class="title">Web-development</h2>
              <h5 class="description">
                WebAplant is a leading web development company 
                delivering complex web projects way beyond regular website building
              </h5>
            </div>
            <div class="md-layout-item md-size-50">
              <h2 class="title">Web-development</h2>
              <h5 class="description">
                WebAplant is a leading web development company 
                delivering complex web projects way beyond regular website building
              </h5>
            </div>
            <div class="md-layout-item md-size-50">
              <h2 class="title">Web-development</h2>
              <h5 class="description">
                WebAplant is a leading web development company 
                delivering complex web projects way beyond regular website building
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
      default: require("@/assets/img/bg7.jpg")
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
