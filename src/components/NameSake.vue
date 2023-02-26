<template>
    <div>HELLO {{ name }}</div>
    <MyMum name="gabriel"/>
</template>

<script>
import MyMum from './MyMum.vue';
export default {
    name: "NameSake",
    props: ["name"],
    components: {
        MyMum,
    }
}
</script>