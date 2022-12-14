<template>
    <main class="cards-container flex">
        <top-card :imgSrc="'/src/assets/images/icon-access-anywhere.svg'"
         :title="title(0)" :context="text(0)" />
        <top-card :imgSrc="'/src/assets/images/icon-security.svg'"
         :title="title(1)" :context="text(1)" />
        <top-card :imgSrc="'/src/assets/images/icon-collaboration.svg'"
         :title="title(2)" :context="text(2)" />
        <top-card :imgSrc="'/src/assets/images/icon-any-file.svg'"
         :title="title(3)" :context="text(3)" />
    </main>
</template>
<script>
import topCard from './top-card.vue';

export default {
    name: 'cards-container',
    props: {
    },
    data() {
        return {
            titles: ['Access your files, anywhere', 'Security you can trust', 'Real-time collaboration', 'Store any type of file'],
            txt: ['The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.', '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.', 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.', 'Whether you\'re sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.']

        }
    },
    methods: {
        title(num) {
            return this.titles[num]
        },
        text(num) {
            return this.txt[num]
        }
    },
    components: {
        topCard
    }
}
</script>
