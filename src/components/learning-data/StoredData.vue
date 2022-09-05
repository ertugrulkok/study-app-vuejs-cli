<template>
  <ul>
    <learning-data
      v-for="data in dataP"
      :key="data.id"
      :title-p="data.title"
      :description-p="data.description"
      :link-p="data.link"
      

    ></learning-data>
  </ul>
</template>
<script>
import LearningData from "./LearningData.vue";
export default {
  components: {
    LearningData,
  },
props:['dataP'],
  data() {
    return {
      
    };
  },
};
</script>
