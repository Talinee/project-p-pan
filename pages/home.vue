<template>
  <div class="table">
    <Table/>
  </div>
</template>
<script>
import axios from 'axios'
import Table from '~/components/Table'

export default {
  components: {
    Table
  },
  data() {
    return {
      newsData: []
    }
  },
  methods: {
    fetchData () {
      axios.get('https://radiant-basin-59716.herokuapp.com/getdata?User_Name=%E0%B9%80%E0%B8%9F%E0%B8%A1&fbclid=IwAR2LaKkoNOZGJ2q0V3d-V3A0rrIEglKu6gI_Dxpghz6y463TfRHFwk6SItg')
      .then(response => {
          this.newsData = response.data
      })
    }
  }, created() {
    this.fetchData()
  }
}
</script>
<style scoped>
</style>
