<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100">
            <h1 class="title">Projects</h1>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="card-expansion">
        <md-card md-with-hover>
          <md-card-header>
            <div class="md-title">Medical project</div>
            <div class="md-subhead">Network of clinics</div>
          </md-card-header>
          <md-card-media>
            <img src="../assets/img/projects/medicine.jpg" alt="Medicine">
          </md-card-media>
          <md-card-expand>
            <md-card-actions md-alignment="space-between">
              <div>
                <md-button class="md-simple md-lg">Learn more</md-button>
              </div>
            </md-card-actions>
            <md-card-expand-content>
              <md-card-content>
                Patient management system for a network of clinics. Automates workflow of medical personel.
              </md-card-content>
            </md-card-expand-content>
          </md-card-expand>
        </md-card>

        <md-card md-with-hover>
          <md-card-header>
            <div class="md-title">Fintech</div>
            <div class="md-subhead">Bank system</div>
          </md-card-header>
          <md-card-media>
            <img src="../assets/img/projects/fintech.jpg" alt="Fintech">
          </md-card-media>
          <md-card-expand>
            <md-card-actions md-alignment="space-between">
              <div>
                <md-button class="md-simple md-lg">Learn more</md-button>
              </div>
            </md-card-actions>
            <md-card-expand-content>
              <md-card-content>
                Bank system with self service functionalities for clients. Automates payment and trading functions.
              </md-card-content>
            </md-card-expand-content>
          </md-card-expand>
        </md-card>

        <md-card md-with-hover>
          <md-card-header>
            <div class="md-title">Document flow</div>
            <div class="md-subhead">Business documents</div>
          </md-card-header>
          <md-card-media>
            <img src="../assets/img/projects/docs.jpg" alt="Documents">
          </md-card-media>
          <md-card-expand>
            <md-card-actions md-alignment="space-between">
              <div>
                <md-button class="md-simple md-lg">Learn more</md-button>
              </div>
            </md-card-actions>
            <md-card-expand-content>
              <md-card-content>
                The system provides services to help companies to manage their everyday's work with documents.
              </md-card-content>
            </md-card-expand-content>
          </md-card-expand>
        </md-card>

        <md-card md-with-hover>
          <md-card-header>
            <div class="md-title md-card-header-whitesmoke">IoT project</div>
            <div class="md-subhead">Communications</div>
          </md-card-header>
          <md-card-media>
            <img src="../assets/img/projects/iot.jpg" alt="Iot">
          </md-card-media>
          <md-card-expand>
            <md-card-actions md-alignment="space-between">
              <div>
                <md-button class="md-simple md-lg">Learn more</md-button>
              </div>
            </md-card-actions>
            <md-card-expand-content>
              <md-card-content>
                Wireless long distance communications through IoT servers and devices automate mechanical tasks.
              </md-card-content>
            </md-card-expand-content>
          </md-card-expand>
        </md-card>
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
      default: require("@/assets/img/headers/virtual-summit.gif")
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
.card-expansion {
    padding: 30px 100px;
  }

  .md-card {
    width: 320px;
    margin: 30px 4px;
    display: inline-block;
    vertical-align: top;
  }

  .md-card-header{
    background-color: whitesmoke !important;
  }
</style>
