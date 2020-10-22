<template>
    <div class="container--overview overview--title">
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