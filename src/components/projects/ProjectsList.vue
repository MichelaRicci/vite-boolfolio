<script>
import ProjectCard from './ProjectCard.vue';
export default {
    name: 'ProjectsList',
    components: { ProjectCard },
    props: { projects: Array }
};
</script>

<template>
    <section id="projects-list" class="my-3">

        <div v-if="projects.length">
            <ProjectCard v-for="project in projects" :key="project.id" :project="project" />
        </div>

    </section>
</template>