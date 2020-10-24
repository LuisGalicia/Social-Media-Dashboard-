<template>
    <div class="container--overview container-subtitle">
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