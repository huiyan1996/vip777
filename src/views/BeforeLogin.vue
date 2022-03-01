<template>
  <div>
        <div class="row mx-0">
            <div class="col-6 px-0">
                <router-link to="/login" class="btn btn-login">Login</router-link>
            </div>
            <div class="col-6 px-0">
                <router-link to="/register" class="btn btn-register">Join Now</router-link>
            </div>
        </div>
  </div>
</template>

<script>

export default {
  name: 'BeforeLogin',
  components: {
  },
  data: function() {
      return {
      }
  }
}
</script>
