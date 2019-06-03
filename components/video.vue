<template>
    <div>
        <h2>{{ path }}</h2>
        <video :src="path" v-video="play"></video>
        <div><button @click="play=!play">{{ state }}</button></div>   
    </div>
</template>

<style scoped>

</style>

<script>
export default {
    data: () => {
        return {
            play: false
        }
    }, 
    directives: {
        video: (el, bind) => {
            bind.value ? el.play() : el.pause();
        }
    }, 
    computed: {
        state: () => {
            // return !this.play ? '再生' : '停止';
            return '再生';
        }, 
    }, 
    props: {
        path: String,
    }
}
</script>
