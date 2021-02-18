<template>
  <div class="note-selectors">
    <NoteSelector v-for="note in notes" :key="note.id" v-bind:note="note" v-bind:selectedNoteId="selectedNoteId" />
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector";

export default {
  data: function() {
    return {
      selectedNoteId: 1,
      notes: [
        { id: 1, body: "This is a first test", timestamp: Date.now() },
        { id: 2, body: "This is a second test", timestamp: Date.now() },
        { id: 3, body: "This is a third test", timestamp: Date.now() },
        { id: 4, body: "This is a fourth test", timestamp: Date.now() },
        { id: 5, body: "This is a fifth test", timestamp: Date.now() },
      ],
    };
  },
  components: {
    NoteSelector,
  },
};
</script>

<style scoped>
.note-selectors {
  flex: 0 0 13em;
}
.note-selectors {
  border-right: 1px solid #dcdadc;
}
</style>
