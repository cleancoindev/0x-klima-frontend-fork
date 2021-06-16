<template>
  <nav>
    <div class="bg-topnav">
      <div class="container-lg p-responsive d-flex mt-2">
        <router-link :to="{ name: 'home' }" class="navbar-brand d-flex align-items-center">
          <h2 class="ticker-name">ω</h2>
          <h1 class="py-4"></h1>
          <h2 class="ticker-name"></h2>
        </router-link>
        <ul>
          <li>
            <div class="mainnav align-items-center">
              <div class="drop-menu-item">
                <h4>Developers</h4>
                <div class="drop-menu-hidden">
                  <a href="https://docs.klima.finance"><p>Documentation</p></a>
                  <a href="https://github.com/klimadao"><p>Github</p></a>
                </div>
              </div>
            </div>
          </li>
          <li>
            <div class="drop-menu-item">
              <h4>Learn</h4>
              <div class="drop-menu-hidden">
                <a href="#what">
                  <p>What is Klima?</p>
                </a>
                <a href="#how">
                  <p>How it works</p>
                </a>
                <a href="https://klimadao.medium.com/">
                  <p>Blog</p>
                </a>
              </div>
            </div>
          </li>
          <li>
            <div class="drop-menu-item">
              <h4>Governance</h4>
              <div class="drop-menu-hidden">
                <a href="http://vote.klima.finance/">
                  <p>Vote</p>
                </a>
                <a href="https://forum.klima.finance">
                  <p>Forum</p>
                </a>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <ModalLogin :open="modalLoginOpen" @close="modalLoginOpen = false" />
  </nav>
</template>

<script>
import { mapState } from 'vuex';

export default {
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
    clickedGetOHM(evt) {
      window.analytics.track('Clicked Button', { button: 'Get OHM' });
    }
  }
};
</script>
