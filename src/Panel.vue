<template>
    <article class="bgf p-fixed o-auto" :class="{
        'x100 h100 xl0 yt0':position==='center', // center
        'x100 y320 xl0 yt0 b-bottom':position==='top', // top
        'x25 h100 xr0 yt0 b-left':position==='right', // right
        'x100 y320 xl0 yb0 b-top':position==='bottom', // bottom
        'x25 h100 xl0 yt0 b-right':position==='left', // left
        }" v-show="show">
        <div class="x92">
            <slot name="panel"></slot>
        </div>
    </article>
</template>
<script>
export default {
    props: ["show", "position"],
    data() {
        return {}
    }
}
</script>
<style scoped></style>