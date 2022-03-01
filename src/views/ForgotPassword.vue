<template>
  <div>
    <BeforeLogin />
    <div class="section">
        <div class="sectionTitle">
            Forgot Password
        </div>

        <div class="row mx-0 mt-3">
            <div class="col-12 px-4">
                <div class="form-group">
                    <label class="form-label">Mobile No.</label>
                    <div class="input-group">
                        <input type="text" class="form-control" v-model="mobileNo">
                    </div>
                </div>
            </div>
        </div>

        <div class="row mt-5 mx-0">
            <div class="col-12 px-4 text-center">
                <button class="btn btn-primary" @click="resetPassword">Reset Password</button>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import BeforeLogin from '@/views/BeforeLogin.vue'

export default {
  name: 'forgotPassword',
  components: {
    BeforeLogin
  },
  data: function() {
    return {
        isShow: false,
        mobileNo: ""
    }
  },
  methods: {
      resetPassword() {
          this.$router.push('/verifyOtp')
      }
  }
}
</script>