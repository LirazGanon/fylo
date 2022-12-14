<template>
<section class="top-card flex">
    <img :src="imgSrc">
    <h3>{{title}}</h3>
    <P>{{context}}</P>
</section>
</template>
<script>
export default {
    name: 'top-container',
    props: {
        imgSrc: String,
        title:String,
        context: String,
    }
}
</script>
