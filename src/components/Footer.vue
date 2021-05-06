<template>
  <footer>
    <div class="footer-row">
      <div class="footer-icon">
        <img src="~/@/assets/logo.svg" class="logo" />
      </div>

      <div class="footer-menu">
        <div class="footer-menu-column">
          <h4>Developers</h4>
          <a href="https://docs.klimafi.finance"><p>Documentation</p></a>
          <a href="https://github.com/klima-fi"><p>Github</p></a>
        </div>
        <div class="footer-menu-column">
          <h4>Learn</h4>
          <a href="#what">
            <p>What is Klima?</p>
          </a>
          <a href="#how">
            <p>How it works</p>
          </a>
          <a href="https://klima.medium.com/">
            <p>Blog</p>
          </a>
        </div>
        <div class="footer-menu-column">
          <h4>Governance</h4>
          <a href="http://vote.klima.finance/">
            <p>Vote</p>
          </a>
          <a href="https://forum.klima.finance">
            <p>Forum</p>
          </a>
        </div>
        <div class="footer-menu-column">
          <h4>Community</h4>
          <a href="https://twitter.com/KlimaFi"><p>Twitter</p></a>
          <a href="https://discord.gg/JWFcg5mCrb"><p>Discord</p></a>
          <a href="https://klima.medium.com/"><p>Blog</p></a>
        </div>
      </div>

      <div class="footer-app-button">
        <router-link
          :to="{ name: 'stake' }"
          class="button button-primary"
          style="color: black !important;"
        >
          Enter App
        </router-link>
      </div>
    </div>
    <ModalLogin :open="modalLoginOpen" @close="modalLoginOpen = false" />
  </footer>
</template>

<script>
import { mapState } from 'vuex';
import { shorten } from '@/helpers/utils';
//import useSound from 'vue-use-sound'
//import buttonSfx from '../assets/stakebutton.mp3'

export default {
  //setup() {d
  //  const [play] = useSound(buttonSfx)

  //  return {
  //    play,
  //  }
  //},
  data() {
    return {
      modalLoginOpen: false
    };
  },
  computed: mapState({
    name: state => state.settings.name,
    address: state => state.settings.address
  }),
  methods: {
    shorten
  }
};
</script>
