
<template>
    <header>
        <h1>{{ title }}</h1>
    </header>
</template>

<script>
export default {
    name: 'Header',
    props: {
        title: String
    }
}
</script>

<style scoped>
    header {
        background-color: #111;
        padding: 20px;
        color: white;
        width: 100%;
        box-sizing: border-box;
      }
    h1 {
        margin: 0;
    }

</style>