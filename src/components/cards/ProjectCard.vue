<template>
  <md-card class="md-card-project" :class="{ 'md-card-hidden': cardHidden }">
    <md-card-media>
      <img src="image" alt="project-image">
    </md-card-media>
    
    <md-card-header :class="getClass(headerColor)">
      <slot name="title"></slot>
      <slot class="subhead"></slot>
    </md-card-header>

    <md-card-content>
      <slot name="description"></slot>
    </md-card-content>

    <md-card-actions>
      <slot name="footer"></slot>
    </md-card-actions>
  </md-card>
</template>

<script>
export default {
  name: "project-card",
  props: {
    headerColor: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      cardHidden: true
    };
  },
  beforeMount() {
    setTimeout(this.showCard, 400);
  },
  methods: {
    showCard: function() {
      this.cardHidden = false;
    },
    getClass: function(headerColor) {
      return "md-card-header-" + headerColor + "";
    }
  }
};
</script>

<style lang="css"></style>
