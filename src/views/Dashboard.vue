<template>
  <div>
    <!-- <Topbar /> -->
    <div class="col-12">
      <DashboardSlider />
    </div>
    <div class="col-12">
      <div class="dashboardMarquee d-flex px-2 py-1">
        <div class="pe-2">
          <font-awesome-icon icon="volume-up" />
        </div>
        <marquee>Welcome to VIP 777</marquee>
      </div>
    </div>
    <BeforeLogin />
    <div class="col-12">
      <GameList />
    </div>
    <div class="col-12">
      <LatestList />
    </div>
    <!-- <BottomNav /> -->
  </div>
</template>

<script>
import DashboardSlider from '@/views/DashboardSlider.vue'
import GameList from '@/views/GameList.vue'
import LatestList from '@/views/LatestList.vue'
import BeforeLogin from '@/views/BeforeLogin.vue'

export default {
  name: 'Dashboard',
  components: {
    DashboardSlider,
    GameList,
    LatestList,
    BeforeLogin
  },
  data: function() {
    return {
      slide: 0
    }
  }
}
</script>