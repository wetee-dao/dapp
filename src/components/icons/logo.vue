<template>
    <svg class="logo-icon" :style="'border-radius: ' + radius + 'px;'" :viewBox="showName ? '0 0 132 29' : '0 0 29 29'" version="1.1"
        xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
        <title>logo</title>
        <g id="home" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
            <g id="Dashboard" transform="translate(-82.000000, -24.000000)" fill="#50FA82" fill-rule="nonzero">
                <g id="header" transform="translate(0.000000, -2.000000)">
                    <g id="编组-2" transform="translate(82.000000, 26.000000)">
                        <g v-show="showName" id="ETEE" transform="translate(39.134957, 4.260000)">
                            <path
                                d="M0,0 L19.8803478,0 L19.8803478,2.64 L2.64,2.64 L2.64,21.12 L19.8803478,21.12 L19.8803478,23.76 L0,23.76 L0,0 Z M3.60417391,10.56 L19.8573913,10.56 L19.8573913,13.2 L5.14226087,13.2 L3.60417391,10.56 Z"
                                id="形状"></path>
                            <polygon id="路径"
                                points="24.1273043 2.64 24.1273043 0 43.9158261 0 42.3777391 2.64 35.330087 2.64 35.330087 23.76 32.690087 23.76 32.690087 2.64">
                            </polygon>
                            <path
                                d="M48.2546087,0 L68.1349565,0 L68.1349565,2.64 L50.8946087,2.64 L50.8946087,21.12 L68.1349565,21.12 L68.1349565,23.76 L48.2546087,23.76 L48.2546087,0 Z M51.8587826,10.56 L68.112,10.56 L68.112,13.2 L53.3968696,13.2 L51.8587826,10.56 Z"
                                id="形状"></path>
                            <path
                                d="M72.3130435,0 L92.1933913,0 L92.1933913,2.64 L74.9530435,2.64 L74.9530435,21.12 L92.1933913,21.12 L92.1933913,23.76 L72.3130435,23.76 L72.3130435,0 Z M75.9172174,10.56 L92.1704348,10.56 L92.1704348,13.2 L77.4553043,13.2 L75.9172174,10.56 Z"
                                id="形状"></path>
                        </g>
                        <g id="编组">
                            <polygon id="路径-2" opacity="0.666480655"
                                points="22.9182073 17.1632653 25.2627451 19.4875696 22.7445378 21.8979592 20.4 19.831911">
                            </polygon>
                            <polygon id="三角形" points="2.73867811e-17 15.3877551 16.4117647 29 0 29"></polygon>
                            <polygon id="路径"
                                points="0 0 7.25981776e-16 10.6278409 20.637883 29 31 29 31 14.0880682 23.0557103 21.5028409 20.896936 19.4431818 31 9.5568182 31 0.247159091 15.5431755 14.5">
                            </polygon>
                        </g>
                    </g>
                </g>
            </g>
        </g>
    </svg>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const props = defineProps(["showName","radius"])
const showName = ref(props.showName)
const radius = ref(props.radius)
</script>

<style lang='scss' scoped>
.logo-icon {
    display: inline-block;
    height: 100%;
    position: relative;
    top: -2px;

    path {
        fill: $primary-text;
    }

    polygon {
        fill: $primary-text;
    }
}
</style>