<template>
    <section class="testimonial-card">
        <p>{{ text }}</p>
        <section class="userDetails">
            <img :src="userImg"/>
            <h6>{{userName}}</h6>
            <p>{{userTitle}}</p>
        </section>
    </section>
</template>
<script>
export default {
    name: 'testimonial-container',
    props: {
        text: String,
        userImg: String,
        userName: String,
        userTitle: String,
    }
}
</script>
