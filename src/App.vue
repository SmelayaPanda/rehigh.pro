<template>
  <v-app class="secondary">
    <v-content>
      <router-view/>
    </v-content>
    <p id="footer_text">Скоро здесь будет новый крутой сайт Re:High Studio!</p>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [{
          icon: 'bubble_chart',
          title: 'Inspire'
        }],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    },
    name: 'App'
  }
</script>
<style lang="scss">
  * {
    box-sizing: border-box;
  }

  html,
  body {
    margin: 0 auto;
    height: 100%;
  }

  body {
    display: flex;
    align-items: center;
    font-family: monospace;
    justify-content: center;
    background-color: darken(#252B37, 4%);
  }

  @mixin backlight($x, $y, $spread, $size, $colorA, $colorB, $duration) {
    &:after {
      position: absolute;
      content: "";
      top: $y;
      left: $x;
      right: 0;
      z-index: -1;
      height: 100%;
      width: 100%;
      margin: 0 auto;
      transform: scale($size);
      -webkit-filter: blur($spread);
      -moz-filter: blur($spread);
      -ms-filter: blur($spread);
      filter: blur($spread);
      background: linear-gradient(270deg, $colorA, $colorB);
      background-size: 200% 200%;
      animation: animateGlow $duration ease infinite;

      @keyframes animateGlow {
        0% {
          background-position: 0% 50%
        }
        50% {
          background-position: 100% 50%
        }
        100% {
          background-position: 0% 50%
        }
      }
    }
  }

  #logo_wrap {
    position: relative;
    width: 440px;
    height: 300px;
    line-height: 30vw;
    text-align: center;
    color: #252B37;
    background-color: #151823;
    animation: textColor 7s ease infinite;
    @include backlight(1, 0vw, 90px, 1.3, #0fffc1, #7e0fff, 7s);

    @keyframes textColor {
      0% {
        color: #7e0fff;
      }
      50% {
        color: #0fffc1;
      }
      100% {
        color: #7e0fff;
      }
    }
  }

  #footer_text {
    text-align: center;
    color: white;
  }

  @media only screen and (max-width: 700px) {
    #logo_wrap {
      width: 220px;
    }
    #footer_text {
      font-size: 11px;
    }
  }
</style>
