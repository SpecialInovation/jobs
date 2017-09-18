<template>
  <div class="data">
    <el-card :body-style="{ padding: '10px' }" v-for="(o, index) in 16" class="data-box" key="{{ o }}">
      <img src="../assets/logo.png" class="image">
      <div style="padding: 14px;">
        <div class="bottom clearfix">
          <span>Airbnb</span>
          <el-button type="text" class="button">Have a Look</el-button>
        </div>
      </div>
    </el-card>
  </div>
</template>

<script>
// const fs = require('fs');

export default {
  name: 'data',
  data() {
    return {
      msg: 'it is data page',
      currentDate: new Date(),
    };
  },
  mounted() {
    // console.log(fs);
    console.log('fafdsfdsa');
    // fs.readFileSync('@/data/enterprise.json');
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .data {
    padding: 0 20px;
  }
  .data-box {
    margin: 1.5%;
    width: 17%;
    float: left;
  }
  .el-card {
    border: 0;
    transition: all 0.2s ease-out;
  }
  .el-card:hover {
    box-shadow: 0 0 8px #888;
  }
  .time {
    font-size: 13px;
    color: #999;
  }
  
  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
      display: table;
      content: "";
  }
  
  .clearfix:after {
      clear: both
  }
</style>
