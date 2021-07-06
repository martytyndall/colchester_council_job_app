<template>
    <header>
        <h1 class="title">{{ title }}</h1>
        
        <h1 class="heading">{{ heading }}</h1>            
    </header>
</template>

<script>

export default{
    name: 'Header',
    props: {
        title: String,
        heading: String,
    },
}
</script>

<style scoped>
    header{
        margin-bottom: 20px;
        letter-spacing: 4px;
        float: left !important;
        width: 100%;
    }

    .title{
        color:lightseagreen;
    }

    .heading{
        width: 800px;
        font-size: 40px;
    }
</style>