<template>
    <header>
        <h1>{{ title }}</h1>
        <HeaderButton text="Add Task" color="green" />
    </header>
</template>

<script>
import HeaderButton from './HeaderButton.vue'

export default {
    name: 'AppHeader',
    props: {
        title: {
            type: String,
            default: 'Hello World'
        }
    },
    components: {
        HeaderButton
    }
}

</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}</style>