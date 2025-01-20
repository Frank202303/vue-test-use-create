<!-- 3 main parts -->

<!--1111111 script: create data -->
<script >
 export default {
  data(){
    return {
      name:"frank",
      status: true,
      statusString: 'pending'
    };
  }
 }
</script>


<!--222222222   template: use data-->
<template>
  <h1>{{ name }}</h1>
  <!-- <p v-if="status">User is acttive</p>
  <p v-else>User is inacttive</p> -->

  <p v-if="statusString === 'active'">User is active</p>
  <p v-else-if="statusString === 'pending'">User is pending</p>
  <p v-else>User is inactive</p>
</template>


<!-- 333333333333333       style -->
<style >

</style>
