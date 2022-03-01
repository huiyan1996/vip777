<template>
  <div>
    <BeforeLogin />
    <div class="section">
        <div class="sectionTitle">
            Validate OTP
            <!-- VerifyOTP -->
        </div>

        <div class="row mt-4 mx-0">
            <div class="col-12 px-4">
                <b class="small">
                    A OTP (One Time Passcode) has been sent to 01161447101 earlier. Please enter the OTP in the field below to verify your phone.
                     <span class="text-danger">OTP will expired in 7m 45s.</span>
                </b>

                <div class="form-group mt-3">
                    <div class="input-group">
                        <input type="text" class="form-control" v-model="otp" placeholder="OTP Code">
                        <span class="input-group-text">Validate OTP</span>
                    </div>
                </div>
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
        otp: ""
    }
  },
  methods: {
      resetPassword() {
          this.$router.push('/verifyOtp')
      }
  }
}
</script>