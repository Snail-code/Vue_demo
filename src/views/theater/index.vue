<template>
    <div class="Mine-container">
        <Header title="我的影院"></Header>
        <router-view></router-view>
        <TabBar></TabBar>
    </div>
</template>

<script>
    import Header from '@/components/Header'
    import TabBar from '@/components/TabBar'
    export default {
        name: "theater",
        components:{
            Header,
            TabBar
        }
    }
</script>

<style scoped>

</style>