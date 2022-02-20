<template>
  <div>
    <div class="bottomNav">
        <router-link to="/" class="bottomNavItem">
            <font-awesome-icon class="icon" icon="home" />
            <span>Home</span>
        </router-link>
        <router-link to="/slotTips" class="bottomNavItem">
            <font-awesome-icon class="icon" icon="lightbulb" />
            <span>Slot Tips</span>
        </router-link>
        <router-link to="/" class="bottomNavItem special">
            <img src="https://ppg668.b-cdn.net/images/liondance.gif" width="100%" alt="">
            <span>Angpau</span>
        </router-link>
        <router-link to="/" class="bottomNavItem">
            <font-awesome-icon class="icon" icon="exchange-alt" />
            <span>History</span>
        </router-link>
        <router-link to="/" class="bottomNavItem">
            <font-awesome-icon class="icon" icon="question" />
            <span>Tutorial</span>
        </router-link>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>
