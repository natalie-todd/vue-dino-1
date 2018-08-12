<template lang='html'>
<div>
   <h2>Job Listings!</h2>
    <ul>
        <li v-for='job in jobs'>{{job.title}}</li>
        </ul> -->
    </div>
    
</template>

<script>
// import image from './assets/g-dino.png';
export default {
  data() {
    return {
      jobs: []
    };
  },
  methods: {
    listingJobs() {
      const JOB_JSON = "../listings.json";
      fetch(JOB_JSON)
        .then(res => res.json())
        .then(result => {
          this.jobs = result;
          console.log(result.title);
        });
    }
  }
};
</script>

<style lang='css'>
</style>
