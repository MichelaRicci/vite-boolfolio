<script>
export default {
  name: 'ProjectCard',
  props: { project: Object },
}
</script>

<template>
  <div class="card m-3">
    <div class="card-header">
      <h2>{{ project.title }}</h2>
    </div>
    <div class="card-body">
      <p>{{ project.description }}</p>
    </div>
    <div class="card-footer d-flex justify-content-between">
      <p>Published on: {{ project.updated_at }}</p>
      <p>By {{ project.slug }}</p>
    </div>
  </div>
</template>