<template>
    <div id="app">
        <keep-alive>
            <router-view v-if="$route.meta.keepAlive"></router-view>
        </keep-alive>
        <router-view v-if="!$route.meta.keepAlive"></router-view>
    </div>
</template>

<script>
    export default {
        name: "app",
        data(){
            return{

            }
        }
    }
</script>

<style>
*{
    margin: 0;
    padding: 0;
}
</style>