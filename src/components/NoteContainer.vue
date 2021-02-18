<template>
  <div class="note-container">
    <NoteSelectors />
    <NoteEditor />
  </div>
</template>

<script>
import NoteSelectors from "./NoteSelectors";
import NoteEditor from "./NoteEditor";

export default {
  components: {
    NoteSelectors,
    NoteEditor,
  },
};
</script>

<style scoped>
.note-container {
  display: flex;
  flex: 1;
}
</style>
