<template>
  <div>
    <BeforeLogin />
    <div class="section">
        <div class="sectionTitle">
            Register
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
                <div class="form-group mt-4">
                    <label class="form-label">How do you know our website?</label>
                    <div class="input-group">
                        <select class="form-control" v-model="howKnow">
                            <option value="">-- Please Select --</option>
                            <option value="1">SMS</option>
                            <option value="2">WHATSAPP</option>
                            <option value="3">Recommend</option>
                            <option value="4">Others</option>
                        </select>
                    </div>
                </div>
                <div class="form-group mt-4">
                    <label class="form-label">Birthday</label>
                    <div class="input-group">
                        <date-picker
                            v-model="dob"
                            format="YYYY-MM-DD"
                            type="date"
                            placeholder="Select date"
                        ></date-picker>
                    </div>
                </div>
                <div class="form-group mt-4">
                    <label class="form-label">Referral Code</label>
                    <div class="input-group">
                        <input type="text" class="form-control" v-model="referral">
                    </div>
                </div>
            </div>
        </div>

        <div class="row mt-4 mx-0">
            <div class="col-12 px-4 text-center">
                <button class="btn btn-primary">Register</button>
            </div>
        </div>

        <div class="row mt-4 mx-0">
            <div class="col-12 px-4 text-center">
                Have account? <router-link to="/login">Login Here</router-link>
            </div>
        </div>

        <div class="sponsor px-4 mt-5">
            <div class="row">
                <div class="col-12">
                    <label>Sponsor for EGames Teams</label>
                </div>
                <div class="col-12">
                    <img src="https://ppg668.b-cdn.net/images/spider.png" />
                    <img src="https://ppg668.b-cdn.net/images/girl.png" />
                </div>
            </div>
            <div class="row mt-3">
                <div class="col-12">
                    <label>Registered &amp; Licensed With</label>
                </div>
                <div class="col-12">
                    <img src="https://ppg668.b-cdn.net/images/pagcor.png" />
                </div>
            </div>
            <div class="row mt-3">
                <div class="col-12">
                    <label>Certified With</label>
                </div>
                <div class="col-12">
                    <img class="mb-2 me-2" src="https://ppg668.b-cdn.net/images/egba.jpg" />
                    <img class="mb-2 me-2" src="https://ppg668.b-cdn.net/images/gamaid.jpg" />
                    <img class="mb-2 me-2" src="https://ppg668.b-cdn.net/images/bmm.png" />
                    <img class="mb-2 me-2" src="https://ppg668.b-cdn.net/images/gamcare.png" />
                </div>
            </div>
            <div class="row mt-3">
                <div class="col-12">
                    <img src="https://ppg668.b-cdn.net/images/18.png" />
                    <img src="https://ppg668.b-cdn.net/images/rg.png"/>
                </div>
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
        password: "",
        howKnow: "",
        dob: "",
        referral: "",
    }
  }
}
</script>