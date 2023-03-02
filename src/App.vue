<template>
  <div>
    <h1>{{ msg }}</h1>

    <TheCard cardTitle="About Me ">
      <template v-slot:default>
        <p>Hi I am Ashadozzaman Shvou</p>
      </template>
      <template v-slot:footer>
        <a href="http://">Learn More</a>
      </template>
    </TheCard>
    <TheCard cardTitle="Apple iPhone 14 Pro">
      <template v-slot:default>
        <img
          src="https://adminapi.applegadgetsbd.com/storage/media/large/iPhone-14-Pro-Max-9907.jpg"
          alt=""
        />
      </template>

      <template v-slot:footer>
        <button>Buy Now</button>
        <button>Add Cart</button>
      </template>
    </TheCard>
    <TheCard cardTitle="Service">
      <u>
        <li>Html</li>
        <li>Slot</li>
        <li>Props</li>
      </u>
    </TheCard>
    <!-- <FirstComponentVue 
            v-for="contact in contacts"
            :key="contact.name"
            :name="contact.name" 
            :website-address="contact.websiteAddress" 
            :phone="contact.phone">
        </FirstComponentVue> -->
  </div>
</template>

<script>
// import FirstComponentVue from './FirstComponent.vue';
import TheCard from "./TheCard.vue";
export default {
  data() {
    return {
      msg: "This is VUE CLI Project",
      contacts: [
        {
          name: "Ashadozzaman",
          phone: "017111111",
          websiteAddress: "ashadozzaman.com",
        },
        {
          name: "Shvou",
          phone: "018111111",
          websiteAddress: "shvoua.com",
        },
        {
          name: "Karim",
          phone: "019111111",
        },
      ],
    };
  },
  components: {
    // FirstComponentVue,
    TheCard,
  },
};
</script>
