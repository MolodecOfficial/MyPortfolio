<script setup lang="ts">

const propsProject = defineProps( {
  image: String,
  name: String,
  link: String,
  code: String
})
</script>

<template>
    <div class="project">
      <img class="project-image" :src="propsProject.image" alt="">
      <p class="project-name"> {{ propsProject.name }} </p>
      <div class="project-info">
        <a class="project-link" :href="propsProject.link"> Demo </a>
        <a class="project-code" :href="propsProject.code"> Code </a>
      </div>
    </div>
</template>

<style scoped>
.project {
  border-radius: 10px;
  width: clamp(150px, 30vw, 300px);
  filter: drop-shadow(0 4px 4px #8e8e8e);
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 8px #8e8e8e);
  }
  & .project-image {
    width: clamp(150px, 30vw, 300px);
    border-radius: 12px;
    height: clamp(50px, 30vw, 150px);
  }
  & .project-info {
    display: flex;
    flex-direction: row;
    gap: clamp(5px, 5vw, 100px);
    margin-bottom: 20px;
    & .project-link {
      font-size: 18px;
      text-decoration: none;
      color: #b5b5b5;
      font-family: Poppins, sans-serif;
      transition: all 0.2s ease-in-out;
      &:hover {
        scale: 1.2;
      }
    }
    & .project-code {
      font-size: 18px;
      text-decoration: none;
      color: #b5b5b5;
      font-family: Poppins, sans-serif;
      transition: all 0.2s ease-in-out;
      &:hover {
        scale: 1.2;
      }
    }
  }
  & .project-name {
    color: wheat;
    font-family: Poppins, sans-serif;
    font-size: 18px;
  }

}
</style>