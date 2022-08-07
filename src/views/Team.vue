<template>
  <div class="wrapper">
    <parallax class="section header-filter" :style="headerStyle">
    </parallax>

    <div class="main main-raised">
        <div class="section text-center">
          <div class="container">
            <h2 class="title">Here is our team</h2>
            <div class="team">
              <div class="md-layout">
                <div class="md-layout-item md-medium-size-33 md-small-size-100">
                  <div class="team-player">
                    <md-card class="md-card-plain">
                      <div class="md-layout-item md-size-50 mx-auto">
                        <img
                          :src="teamImg1"
                          alt="Thumbnail Image"
                          class="img-raised rounded-circle img-fluid"
                        />
                      </div>
                      <h4 class="card-title">
                        Alibek
                        <br />
                        <small class="card-description text-muted">CEO</small>
                      </h4>

                      <md-card-actions class="text-center">
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-twitter"></i>
                        </md-button>
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-instagram"></i>
                        </md-button>
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-facebook-square"></i>
                        </md-button>
                      </md-card-actions>
                    </md-card>
                  </div>
                </div>
                <div class="md-layout-item md-medium-size-33 md-small-size-100">
                  <div class="team-player">
                    <md-card class="md-card-plain">
                      <div class="md-layout-item md-size-50 mx-auto">
                        <img
                          :src="teamImg2"
                          alt="Thumbnail Image"
                          class="img-raised rounded-circle img-fluid"
                        />
                      </div>
                      <h4 class="card-title">
                        Malika
                        <br />
                        <small class="card-description text-muted"
                          >CTO</small
                        >
                      </h4>

                      <md-card-actions class="text-center">
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-twitter"></i>
                        </md-button>
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-linkedin"></i>
                        </md-button>
                      </md-card-actions>
                    </md-card>
                  </div>
                </div>
                <div class="md-layout-item md-medium-size-33 md-small-size-100">
                  <div class="team-player">
                    <md-card class="md-card-plain">
                      <div class="md-layout-item md-size-50 mx-auto">
                        <img
                          :src="teamImg3"
                          alt="Thumbnail Image"
                          class="img-raised rounded-circle img-fluid"
                        />
                      </div>
                      <h4 class="card-title">
                        Aigerim
                        <br />
                        <small class="card-description text-muted">CDO</small>
                      </h4>

                      <md-card-actions class="text-center">
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-twitter"></i>
                        </md-button>
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-instagram"></i>
                        </md-button>
                        <md-button
                          href="javascript:void(0)"
                          class="md-just-icon md-simple"
                        >
                          <i class="fab fa-facebook-square"></i>
                        </md-button>
                      </md-card-actions>
                    </md-card>
                  </div>
                </div>
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
      default: require("@/assets/img/persons/Alibek.jpg")
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
