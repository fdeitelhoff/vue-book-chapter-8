<template>
  <div>
    <img v-bind:src="image" />
    <br />
    <a target="_blank" :href="url">Ich bin ein Link</a>
  </div>
</template>

<script>
export default {
  name: 'Binding',
  data: () => {
    return {
      image: 'https://dpunkt.de/wp-content/uploads/2019/07/logo.svg',
      url: 'https://www.dpunkt.de',
    };
  },
};
</script>
