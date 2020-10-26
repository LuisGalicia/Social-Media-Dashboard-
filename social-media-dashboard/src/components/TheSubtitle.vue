<template>
    <div class="container__overview">
        {{ titulo }}
    </div>
</template>

<script>
    export default {
        name: 'TheSubtitle',
        props : {
            titulo: String
        }
    }
</script>