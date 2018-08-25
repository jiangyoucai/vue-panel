<template>
    <div>
        <p>v-panel</p>
        <v-panel :show="show" :position="'center'">
            <div slot="panel">
                <div class="x100">
                    <p class="container ym20 x-between">
                        <span class="b-title">产品信息</span>
                        <span @click="show = 0">X</span>
                    </p>
                </div>
            </div>
        </v-panel>
    </div>
</template>
<script>
export default {
    data() {
        return {
            show: 1
        }
    }
}
</script>
<style scoped></style>