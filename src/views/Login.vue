<template>
  <div>
    <BeforeLogin />
    <div class="section">
        <div class="sectionTitle">
            Login
        </div>

        <div class="row mx-0">
            <div class="col-12 px-4">
                <div class="form-group">
                    <label class="form-label">Mobile No.</label>
                    <div class="input-group">
                        <input type="text" class="form-control" v-model="mobileNo">
                    </div>
                </div>
                <div class="form-group mt-4">
                    <label class="form-label">Password</label>
                    <div class="input-group">
                        <input :type="isShow?'text':'password'" class="form-control" v-model="password">
                        <span class="input-group-text" @click="isShow=!isShow"><font-awesome-icon :icon="isShow?'eye-slash':'eye'" /></span>
                    </div>
                </div>
            </div>
        </div>

        <div class="row mt-5 mx-0">
            <div class="col-12 px-4 text-center">
                <button class="btn btn-primary">Login</button>
            </div>
        </div>

        <div class="row mt-4 mx-0">
            <div class="col-12 px-4 text-center">
                <router-link to="/forgotPassword" class="forgotPasswordLink">Forgot Password</router-link>
            </div>
        </div>

        <div class="row mt-2 mx-0">
            <div class="col-12 px-4 text-center">
                Join us now! <router-link to="/register">Register</router-link>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import BeforeLogin from '@/views/BeforeLogin.vue'

export default {
  name: 'Login',
  components: {
    BeforeLogin
  },
  data: function() {
    return {
        isShow: false,
        mobileNo: "",
        password: ""
    }
  }
}
</script>