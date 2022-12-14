<template>
    <main class="testimonial-container">
        <testimonial-card :userImg="'/src/assets/images/profile-1.jpg'"
         :text="text(0)" :userName="userName(0)" :userTitle="userTitle(0)" />
        <testimonial-card :userImg="'/src/assets/images/profile-2.jpg'"
         :text="text(1)" :userName="userName(1)" :userTitle="userTitle(1)" />
         <testimonial-card :userImg="'/src/assets/images/profile-3.jpg'"
         :text="text(2)" :userName="userName(2)" :userTitle="userTitle(2)" />
      
    </main>
</template>
<script>
import TestimonialCard from './testimonial-card.vue'

export default {
    name: 'cards-container',
    props: {
    },
    data() {
        return {
        texts:['Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.','Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.','Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.'],
        userNames:['Satish Patel','Bruce McKenzie','Iva Boyd'],
        userTitles:['Founder & CEO, Huddle','Founder & CEO, Huddle','Founder & CEO, Huddle']    
        }
    },
    methods: {
        text(num) {
            return this.texts[num]
        },
        userName(num) {
            return this.userNames[num]
        },
        userTitle(num) {
            return this.userTitles[num]
        },
    },
    components: {
        TestimonialCard
    }
}
</script>
