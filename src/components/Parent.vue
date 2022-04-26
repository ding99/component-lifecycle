<template>
    <div>
        Parent component
    </div>
</template>

<script>
    export default {
        name: 'LifecycleParent',
        beforeCreate() {
            console.log ('Parent beforeCreated()')
        },
        created() {
            console.log ('Parent created()')
        },
        beforeMount() {
            console.log ('Parent beforeMount()')
        },
        mounted () {
            console.log ('Parent mounted()')
        },
        beforeUpdate () {
            console.log ('Parent beforeUpdate()')
        },
        updated () {
            console.log ('ChParentild Updated()')
        },
        beforeUnmount () {
            console.log ('Parent beforeUnmount()')
        },
        unmounted () {
            console.log ('Parent unmounted ()')
        }
    }
</script>

<style scoped>

</style>