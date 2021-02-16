<template>
    <div>
        <h1>Output List</h1>
    </div>
</template>
<script>
import Vue from 'vue';
import axios from 'axios'
import VueAxios from 'vue-axios'
Vue.use(VueAxios, axios)
export default {
    name:"output-list",
    mounted()
    {
        Vue.axios.get('http://127.0.0.1:1337/multi/55')
        .then((resp)=>{
            console.warn(resp)
        })
    }
}
</script>