<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{ name: 'JobDetails', params: { id: job.id}}">
      <h1>{{ job.title }}</h1>
    </router-link>
  </div>

</template>

<script>
export default {
  data(){
    return{
        jobs: [
            { title: 'UX Designer', id: 1, details: 'jorem'},
            { title: 'Web developer', id: 2, details: 'dorem'},
            { title: 'Vue developer', id: 3, details: 'borem'},
        ]
    }
  }
}
</script>

<style>
 a{
  text-decoration: none;
 }
</style>