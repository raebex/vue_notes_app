<template>
  <div
    class="note-selector"
    v-bind:class="{ active: selectedNoteId === note.id }"
  >
    <p class="note-selector-title">{{ note.body }}</p>
    <p class="note-selector-timestamp">{{ note.timestamp }}</p>
  </div>
</template>

<script>
export default {
  props: ["note", "selectedNoteId"],
};
</script>

<style scoped>
.note-selector {
  padding: 1em;
}
.note-selector p {
  margin: 0;
}
.note-selector {
  border-bottom: 1px solid #dcdadc;
}
.note-selector.active {
  background-color: #fce18d;
}
.note-selector-title {
  background-color: inherit;
}
.note-selector-timestamp {
  color: #626262;
  background-color: inherit;
}
.note-selector-title {
  font-weight: bold;
}
.note-selector-timestamp {
  font-size: 0.7em;
}
</style>
