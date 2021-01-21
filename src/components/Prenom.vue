<template>
  <h3>Mon nom est Léa {{ nom }}</h3>
</template>

<script>
export default {
  props: {
    nom: String,
  },
};
</script>