<template>
  <div>
    <div class="topPart">
      <b-icon class="burgerMenu" icon="list" @click="openSideMenu=!openSideMenu" />
      <img src="https://ppg668.b-cdn.net/images/logo_sm.gif" width="220px" alt="">
      <b-dropdown class="langSel" right text="EN" variant="primary" toggle-class="langDropdown">
        <b-dropdown-item>EN</b-dropdown-item>
        <b-dropdown-item>CN</b-dropdown-item>
      </b-dropdown>
    </div>
    <div class="sideDisplay" :class="{open: openSideDisplay}" @click="openSideDisplay=!openSideDisplay">
      <img src="https://ppg668.b-cdn.net/images/float2.png" class="sideToggle">
      <div class="sideContent">
        <div class="icon whatsapp"><font-awesome-icon :icon="['fab', 'whatsapp']" /></div>
        <div>EMERGENCY HOTLINE WHATSAPP</div>
        <div>+60179317665</div>
        <div class="icon telegram mt-3"><font-awesome-icon :icon="['fab', 'telegram']" /></div>
        <div>TELEGRAM CHANNEL</div>
      </div>
    </div>
    <div class="sideMenuOverlay" v-if="openSideMenu" @click="openSideMenu=!openSideMenu"></div>
    <div class="sideMenu" :class="{open:openSideMenu}">
      <div class="sideMenuLogo">
        <img src="https://ppg668.b-cdn.net/images/logo.png" width="100%">
      </div>
      <div class="sideMenuWrapper">
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="home" />
          <span>Home</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="dollar-sign" />
          <span>Deposit</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="money-bill-alt" />
          <span>Withdraw</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="sitemap" />
          <span>Agent</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="lightbulb" />
          <span>Slot Tips</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="lock" />
          <span>Login</span>
        </router-link>
        <router-link to="/" class="sideMenuItem">
          <font-awesome-icon class="icon" icon="user-edit" />
          <span>Join Now</span>
        </router-link>
      </div>
    </div>
    <div class="treasureBox" v-if="treasureBox">
      <div class="closeBtn">
        <font-awesome-icon icon="times-circle" @click="treasureBox=!treasureBox" />
      </div>
      <img src="https://ppg668.b-cdn.net/images/wheel.gif">
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data: function() {
    return {
      openSideDisplay: false,
      openSideMenu: false,
      treasureBox: true,
    }
  }
}
</script>
