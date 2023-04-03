<template>
  <img :alt="name" loading="lazy" :src="getFullUrl(imgSrc)" />
</template>

<script lang="ts">
export default {
  name: "GalleryImage",
  props: {
    name: String,
    imgSrc: {
      type: String,
      required: true,
    },
  },
  methods: {
    getFullUrl: function (relativeUrl: string) {
      return new URL(relativeUrl, import.meta.url).href;
    },
  },
};
</script>
