<template>
  <div>
    <Topbar />
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
    <div class="row mx-0">
      <div class="col-6 px-0">
        <router-link to="/login" class="btn btn-login">Login</router-link>
      </div>
      <div class="col-6 px-0">
        <router-link to="/register" class="btn btn-register">Join Now</router-link>
      </div>
    </div>
    <div class="col-12">
      <GameList />
    </div>
    <div class="col-12">
      <LatestList />
    </div>
    <BottomNav />
  </div>
</template>

<script>
import Topbar from '@/views/Topbar.vue'
import DashboardSlider from '@/views/DashboardSlider.vue'
import GameList from '@/views/GameList.vue'
import LatestList from '@/views/LatestList.vue'
import BottomNav from '@/views/BottomNav.vue'

export default {
  name: 'Dashboard',
  components: {
    Topbar,
    DashboardSlider,
    GameList,
    LatestList,
    BottomNav,
  },
  data: function() {
    return {
      slide: 0
    }
  }
}
</script>