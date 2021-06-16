<template>
  <div class="column">
    <!--<Nav />-->

    <div class="block hero">
      <div class="d-flex flex-column side-menu" style="position:absolute; right: 15px">
        <a href="https://klimadao.medium.com/" target="_blank" class="pb-4">
          <img
            src="~/@/assets/medium.svg"
            alt=""
            class="social-icon-small"
            style="height: 25px; width: 25px;"
          />
        </a>
        <a href="https://twitter.com/klimadao" target="_blank" class="pb-4">
          <img
            src="~/@/assets/twitter.svg"
            alt=""
            class="social-icon-small"
            style="height: 25px; width: 25px;"
          />
        </a>
        <a href="https://discord.gg/wBTsKXWDEU" target="_blank" class="pb-4">
          <img
            src="~/@/assets/discord.svg"
            alt=""
            class="social-icon-small"
            style="height: 25px; width: 25px;"
          />
        </a>
      </div>
      <div style="margin: 2rem auto 0 0">
        <h1 style="padding: 30px">Klima</h1>
        <p class="hero-desc">
          A new community that’s resolute on solving climate change by creating a black hole for carbon which will suck carbon credits out of the default world and collateralize a carbon backed currency.
        </p>
        <div class="hero-icon">
          <img
                  src="~/@/assets/KlimaDAO/KlimaLogo_Transparent.png"
                  alt=""
                  class="social-icon-small"
                  style="height: 100px; width: 100px; filter: none"
          />
        </div>
        <h3 style="text-align: center;">Sign up for updates</h3>
        <div style="text-align: center">
          <router-link
                  :to="{ name: 'home' }"
                  style="margin:1rem auto;max-width:200px; color: black !important; width: 100%"
                  class="button button-primary"
          >
            Register
          </router-link>
        </div>
        <p class="hero-desc">
          Klima is an Algorithmic Climate Protocol. Klima DAO utilizes Protocol Owned Value to enable carbon (CO2e) price consistency and scarcity within an infinite carbon supply system.
        </p>
      </div>


    </div>
    <!--<div class="block">
      <div class="row-responsive flex-centered" id="what">
        <h3 class="centered-text py-8">Klima DAO Is</h3>
      </div>


      <div class="row-responsive flex-centered">
        <div class="feature-box-module" style="">
          <div class="feature-block-image">
            <img src="~/@/assets/Backedbyassets-banner.png" alt="" />
          </div>
          <div class="feature-block-desc">
            <h3>Backed by Assets</h3>
            <p>
              Every KLIMA is backed by a VCU20 and KLIMA-VCU20 LP in the treasury. This intrinsic value cannot
              be diluted, providing a fundamental check on inflation and check on infinite "climate" greenification
            </p>
          </div>
        </div>
        <div class="feature-box-module" style="">
          <div class="feature-block-image">
            <img src="~/@/assets/Algo&#45;&#45;banner.png" alt="" />
          </div>
          <div class="feature-block-desc">
            <h3>Algorithmically Managed</h3>
            <p>
              Klima DAO has an adjustable policy state, allowing the DAO to adjust parameters and
              algorithmically optimize for stability or growth.
            </p>
          </div>
        </div>
        <div class="feature-box-module" style="">
          <div class="feature-block-image">
            <img src="~/@/assets/community-banner.png" alt="" />
          </div>
          <div class="feature-block-desc">
            <h3>Community Governed</h3>
            <p>
              Klima DAO is a DAO first project actively working toward complete distribution of the
              system to the community. Climate Governance is a public good after all.
            </p>
          </div>
        </div>
      </div>
    </div>


    <div class="block row-responsive no-pad">
      <div class="row-flex-max feature-row py-9">
        <div class="row-flex-desc">
          <h2>What makes Klima unique?</h2>
          <p>
            Klima is a floating algorithmic climate currency. This means that it has mechanisms to promote
            stability and predictablility without directly pegging to any asset. This is to build in strong accountability into carbon markets using this mechanism
          </p>
          <p>
            Klima Pistós - Climate Loyal
          </p>
          <p>
            The slogan lifted from the US Marine Corp "Semper Fi", implies that the entire premise of the DAO is only 1.
            Climate over everything. It remains the mantra for how governance is decided and how all decisions get made
          </p>
        </div>
      </div>
      <div class="row-flex-image feature-image">
        <img src="~/@/assets/olympus1.svg" alt="" />
      </div>
    </div>

    <div class="block">
      <div class="row-responsive flex-centered mb-9" id="how">
        <h1 class="centered-text">How It Works</h1>
      </div>



      <div class="row-responsive flex-centered">
        <div class="works-module-responsive">
          <div class="works-icon"><img src="~/@/assets/features/reserves.svg" alt="" /></div>
          <div class="works-desc">
            <h3>Climate Reserves</h3>
            <p>
              KLIMA is always backed by one VCU20 or one KLIMA backed by one VCU20. This creates a
              demand-based constraint on issuance of supply.
            </p>
          </div>
        </div>
        <div class="works-module-responsive">
          <div class="works-icon"><img src="~/@/assets/features/marketops.svg" alt="" /></div>
          <div class="works-desc">
            <h3>Market Operations</h3>
            <p>
              New KLIMA is created via direct sales into the market. These sales increase linearly
              with the market premium and produce profits for stakers.
            </p>
          </div>
        </div>
      </div>
      <div class="row-responsive flex-centered">
        <div class="works-module-responsive">
          <div class="works-icon"><img src="~/@/assets/features/governance.svg" alt="" /></div>
          <div class="works-desc">
            <h3>Governance</h3>
            <p>
              The KLIMA controls policy tools that allow us to loosen, increasing profitability and
              volatility, or tighten, increasing stability and predictability.
            </p>
          </div>
        </div>
        <div class="works-module-responsive">
          <div class="works-icon"><img src="~/@/assets/features/bonding.svg" alt="" /></div>
          <div class="works-desc">
            <h3>Bonding</h3>
            <p>
              New KLIMA is created via deferred sales for LP. Bonders lock their LP for a vesting term
              and receive a discount on KLIMA when the trade ultimately occurs.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="block row-responsive no-pad">
      <div class="row-flex-image feature-image">
        <img src="~/@/assets/olympus2.svg" alt="" />
      </div>

      <div class="row-flex-max feature-row">
        <div class="row-flex-desc">
          <h2>A world of opportunity</h2>
          <p>
            The Klima carbon reserve system enables new implementations of a multitude of DeFi
            climate primitives. While it's foundation is built on carbon markets. The potential to expand to other types
            of social asset classes like blue carbon markets, social credits, equality financing, ecosystem services pricing is within reach. The opportunity to finance the safekeeping of our planet remains possible with KLIMA.
          </p>
        </div>
      </div>
    </div>

    <Footer />-->
  </div>
</template>

<script>
import { mapState } from 'vuex';

export default {
  data() {
    return {
      form: {
        quantity: ''
      },
      modalLoginOpen: false
    };
  },
  computed: {
    ...mapState(['settings']),
    isValid() {
      return parseFloat(this.form.quantity);
    },
    maxStrike() {
      const exchangeRate = this.settings.exchangeRates[this.form.asset];
      return exchangeRate && exchangeRate.usd ? exchangeRate.usd : 1e9;
    }
  },
  methods: {}
};
</script>
<style scoped>
.hasEffect {
  cursor: pointer;
}
</style>
