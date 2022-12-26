<template>
<div>
  <H1>SALAH EDDINE FILE JSON READER AXIOS API</H1>

<H2>"{{ SALAHTEST }}"</H2>

</div>
</template>

<script>
import axios from 'axios'
import { ref } from 'vue';
export default{
  setup (){
const SALAHTEST = ref('')

    axios.get('https://mocki.io/v1/d9bc6bf6-892f-4ecf-b59f-74f37fb71647')
    .then(response =>{
      SALAHTEST.value= response.data.CAR
    })
    return{
      SALAHTEST
    }
  }
}

</script>