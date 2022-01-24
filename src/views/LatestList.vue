<template>
  <div>
    <carousel :per-page="1" :mouse-drag="true" paginationColor="#fff" paginationActiveColor="#fee577">
        <slide>
            <div class="latestList">
                <div class="listTitle">Latest Deposits</div>
                <CustomTable :thArray="depositThArray" :data="depositData" />
            </div>
        </slide>
        <slide>
            <div class="latestList">
                <div class="listTitle">Latest Withdrawal</div>
                <CustomTable :thArray="withdrawThArray" :data="withdrawData" />
            </div>
        </slide>
    </carousel>
  </div>
</template>

<script>
import CustomTable from '@/components/CustomTable.vue'
export default {
  name: 'LatestList',
  components: {
      CustomTable
  },
  data: function() {
      return {
          depositThArray: [
              "Member",
              "RM",
              "Date"
          ],
          depositData: [
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"}
          ],
          withdrawThArray: [
              "Member",
              "RM",
              "Date"
          ],
          withdrawData: [
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"},
              {member: "+601******0229", amt: "RM530.00", date: "2022-01-25 04:04:30"}
          ]
      }
  }
}
</script>
