<template lang='html'>
<div class=''>
    <img src='../assets/g-dino.png' alt='dino logo'>
    </div>
    
</template>

<script>
// import image from './assets/g-dino.png';
export default {
    data() {
        return {
            jobs: [],
        };
    },
    methods: {
        listingJobs() {
            const JOB_JSON = './listings.json';
            fetch(JOB_JSON)
            .then(res => res.json())
            .then (result => {
                this.jobs = result
                console.log(result.title)
            })
        },
    },
};
</script>

<style lang='css'>
</style>
