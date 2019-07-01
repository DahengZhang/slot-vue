<template>
    <div class="component-list-wrapper">
        <p>This is list wrapper</p>
        <slot :list="data"></slot>
    </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array|Object,
            required: true
        }
    }
}
</script>
