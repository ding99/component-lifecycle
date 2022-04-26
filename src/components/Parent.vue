<template>
    <div>
        Parent component
        <button @click="showChild = !showChild">Toggle Child</button>
        <LifecycleChild v-if="showChild" />  
    </div>
</template>

<script>
    import LifecycleChild from './Child.vue'
    export default {
        components: { LifecycleChild },
        name: 'LifecycleParent',
        data () {
            return {
                showChild: true,
            }
        },
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