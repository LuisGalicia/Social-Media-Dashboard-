<template>
    <div>
        <div>
           <h1>{{ titulo }}</h1> 
           <h4>{{ subtitulo }}</h4>
        </div>
        <div>
            <p>Dark mode</p>
           <label>
            <input type="checkbox">
            <span></span>
        </label> 
        </div>
        
    </div>
</template>

<script>
    export default {
        name: 'TheHeading',
        props: {
            titulo: String,
            subtitulo: String
        }
    }
</script>