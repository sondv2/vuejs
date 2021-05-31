<template>
    <footer>
        <h1>{{ textFooter }}</h1>
    </footer>
</template>

<script>
export default {
    name: 'comp-footer',
    props: {
        title: String,
        default: 'Gia tri mac dinh'
    },
    data() {
        return {
            textFooter: 'Hello Footer'
        }
    }
}
</script>

<style>

</style>
