<template>
    <div>Example Component, {{ greeting }}</div>
    <div>Foo: {{ foo }}</div>
</template>

<script>
import {ref} from 'vue'
export default {
    props: ['foo'],
    setup() {
       const greeting= ref('Component setup');
       return {
           greeting
       }
    }
}
</script>
