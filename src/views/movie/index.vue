<template>
    <div class="Movie-container">
        <Header title="我的电影"></Header>
        <!-- Standard button -->
        <button type="button" class="btn btn-default">（默认样式）Default</button>

        <!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
        <button type="button" class="btn btn-primary">（首选项）Primary</button>

        <!-- Indicates a successful or positive action -->
        <button type="button" class="btn btn-success">（成功）Success</button>

        <!-- Contextual button for informational alert messages -->
        <button type="button" class="btn btn-info">（一般信息）Info</button>

        <!-- Indicates caution should be taken with this action -->
        <button type="button" class="btn btn-warning">（警告）Warning</button>

        <!-- Indicates a dangerous or potentially negative action -->
        <button type="button" class="btn btn-danger">（危险）Danger</button>

        <!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
        <button type="button" class="btn btn-link">（链接）Link</button>
        <router-view></router-view>
        <TabBar></TabBar>
    </div>
</template>

<script>
    import Header from '@/components/Header'
    import TabBar from '@/components/TabBar'
    export default {
        name: "index",
        components:{
            Header,
            TabBar
        }
    }
</script>

<style lang="scss" scoped>
    .active{
        color: #fe4365;
    }
    .Movie-container {
        width: 100%;
        height: 100%;
        overflow: hidden;
        -moz-box-sizing: border-box;
        padding-bottom: 50px;
        box-sizing: border-box;
        nav {
            height: 46px;
            line-height: 46px;
            background-color: #ffffff;
            display: flex;
            justify-content: space-around;
            border-bottom: 1px solid #e6e6e6;
            span {
                font-size: 15px;
                font-weight: 600;
                flex: 1;
                text-align: center;
                cursor: pointer;
            }
            .city {
            }
            .icon {
                font-size: 20px;
            }
        }
    }
</style>