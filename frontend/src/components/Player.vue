<script>
export default {
  props: ["id"],
  computed: {
    videoSrc() {
      return "http://localhost:1337/api/medias/play/" + this.id;
    },
  },
};
</script>
<template>
  <div>
    <video class="w-100" :src="videoSrc" controls>
      Your browser does not support the video tag.
    </video>
  </div>
</template>
