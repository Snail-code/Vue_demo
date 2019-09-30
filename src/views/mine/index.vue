<template>
    <div class="Movie-container">
        <Header title="我的信息"></Header>
        <router-view></router-view>
        <TabBar></TabBar>
    </div>
</template>

<script>
    import Header from '@/components/Header'
    import TabBar from '@/components/TabBar'
    export default {
        name: "mine",
        components:{
            Header,
            TabBar
        }
    }
</script>

<style scoped>

</style>