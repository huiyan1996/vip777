<template>
  <div>
    <table class="table">
        <thead>
            <tr>
                <th v-for="(v, k) in thArray" :key="k">{{v}}</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="(v, k) in data" :key="k">
                <td v-for="(v1, k1) in v" :key="k1">{{v1}}</td>
            </tr>
        </tbody>
    </table>
  </div>
</template>

<script>

export default {
  name: 'GameList',
  components: {
  },
  props: {
      thArray: Array,
      data: Array
  }
}
</script>
