<template>
  <div>
      <div class="gameNav">
          <div class="gameNavItem" :class="{active: currentList=='slot'}" @click="currentList='slot'">
              <img src="https://ppg668.b-cdn.net/images/selector/slot.png" alt="">
              <span>Slot</span>
          </div>
          <div class="gameNavItem" :class="{active: currentList=='casino'}" @click="currentList='casino'">
              <img src="https://ppg668.b-cdn.net/images/selector/live.png" alt="">
              <span>Live Casino</span>
          </div>
          <div class="gameNavItem" :class="{active: currentList=='fish'}" @click="currentList='fish'">
              <img src="https://ppg668.b-cdn.net/images/selector/fish.png" alt="">
              <span>Fish Hunt</span>
          </div>
          <div class="gameNavItem" :class="{active: currentList=='sport'}" @click="currentList='sport'">
              <img src="https://ppg668.b-cdn.net/images/selector/sport.png" alt="">
              <span>Sports</span>
          </div>
          <div class="gameNavItem special">
              <img src="https://ppg668.b-cdn.net/images/selector/promo.gif" alt="">
              <span>Promotions</span>
          </div>
      </div>
      <div class="col-12">
          <div class="row mx-0">
              <div class="col-6"><img class="gpic_918kiss" src="https://ppg668.b-cdn.net/images/slot/918kiss.png" width="100%"></div>
              <div class="col-6"><img class="gpic_mega888" src="https://ppg668.b-cdn.net/images/slot/mega888.png" width="100%"></div>
              <div class="col-6"><img class="gpic_pussy888" src="https://ppg668.b-cdn.net/images/slot/pussy888.png" width="100%"></div>
              <div class="col-6"><img class="gpic_pragmatic" src="https://ppg668.b-cdn.net/images/slot/pragmatic.png" width="100%"></div>
              <div class="col-6"><img class="gpic_918kaya" src="https://ppg668.b-cdn.net/images/slot/918kaya.png" width="100%"></div>
              <div class="col-6"><img class="gpic_evo888" src="https://ppg668.b-cdn.net/images/slot/evo888.png" width="100%"></div>
              <div class="col-6"><img class="gpic_joker123" src="https://ppg668.b-cdn.net/images/slot/joker123.png" width="100%"></div>
              <div class="col-6"><img class="gpic_scr888" src="https://ppg668.b-cdn.net/images/slot/scr888.png" width="100%"></div>
              <div class="col-6"><img class="gpic_xe88h5" src="https://ppg668.b-cdn.net/images/slot/xe88h5.png" width="100%"></div>
              <div class="col-6"><img class="gpic_playtech" src="https://ppg668.b-cdn.net/images/slot/playtech.png" width="100%"></div>
              <div class="col-6"><img class="gpic_asiagaming" src="https://ppg668.b-cdn.net/images/slot/asiagaming.png" width="100%"></div>
              <div class="col-6"><img class="gpic_bbinf" src="https://ppg668.b-cdn.net/images/slot/bbinf.png" width="100%"></div>
          </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'GameList',
  components: {
  },
  data: function() {
      return {
          currentList: "slot"
      }
  }
}
</script>
