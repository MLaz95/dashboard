<template>
    <div
    v-for="n in test"
    class="my_card bg-danger border border-black col p-3 text-center"
    >
        <div class="border rounded-3 h-100 d-flex flex-column justify-content-around">
            <div>{{ n }}</div>
            <div>{{ n }}</div>
        </div>
    </div>
</template>

<style>
.my_card {
    height: 200px;

}
</style>

<script>
    export default{
        data(){
            return{
                test: [1,2,3,4,5,6]
            }
        }
    }
</script>