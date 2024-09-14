<script>
    import { defineComponent } from 'vue';
    import navbar from "./components/navbar.vue"
    import home from "./components/home.vue"
    import about from "./components/about.vue"
    import services from "./components/services.vue"
    import skill from "./components/skill.vue"
    import resume from "./components/resume.vue"
    import contact from "./components/contact.vue"
    export default defineComponent ({
        components: {navbar, home, about, services, skill, resume, contact}
    })
</script>

<template>
    <navbar class="overflow-hidden" />
    <home class="overflow-hidden" />
    <about class="overflow-hidden" />
    <services class="overflow-hidden" />
    <skill class="overflow-hidden" />
    <resume class="overflow-hidden" />
    <contact class="overflow-hidden" />
</template>