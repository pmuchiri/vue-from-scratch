<template>
     <div>
        <p>{{ item.title }}</p>
        <p @click="toggle = ! toggle">Details</p>
        <p v-if="toggle">{{ item.description }}</p>
        <!-- allows toggling in the details tab to provide description...click on/off on details tab to test -->
    </div>
    
</template>

<script>
    export default {
        name: "Accordion",
       
        props: ['item'],

        data: function () {
            return {
                toggle: false,
            }
        }
    }

</script>

