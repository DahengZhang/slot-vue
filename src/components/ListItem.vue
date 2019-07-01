<template>
    <div class="component-list-item">
        <strong>{{ data.name }}</strong>
        <p>{{ data.value }}</p>
    </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Object,
            required: true
        }
    }
}
</script>
