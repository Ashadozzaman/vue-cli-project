<template>
    <div>
        <h1>{{msg}}</h1>
        <FirstComponentVue 
            v-for="contact in contacts"
            :key="contact.name"
            :name="contact.name" 
            :website-address="contact.websiteAddress" 
            :phone="contact.phone">
        </FirstComponentVue>
    </div>
</template>

<script>
import FirstComponentVue from './FirstComponent.vue';
export default {
    data(){
        return {
            msg: "This is VUE CLI Project",
            contacts:[
                {
                    name: 'Ashadozzaman',
                    phone: "017111111",
                    websiteAddress: "ashadozzaman.com"

                },
                {
                    name: 'Shvou',
                    phone: "018111111",
                    websiteAddress: "shvoua.com"

                },
                {
                    name: 'Karim',
                    phone: "019111111",

                },
            ]
        };
    },
    components:{
        FirstComponentVue
    }
}
</script>