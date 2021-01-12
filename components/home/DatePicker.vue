<template>
    <no-ssr>
    <b-datepicker v-model="selectedDate" 
        inline 
        :unselectable-days-of-week="[0, 6]">
    </b-datepicker>
    </no-ssr>
</template>

<script>
    export default {
        data() {
            return {
                selectedDate: new Date()
            }
        }
    }
</script>
