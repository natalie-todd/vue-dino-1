<template lang='html'>
<div class=''>
    <ul>
        <li v-for='job in jobs'>{{job.title}}</li>
        </ul>
    </div>
    
</template>

<script>
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
                console.log(result)
            })
        }
    }
}
</script>

<style>
</style>
