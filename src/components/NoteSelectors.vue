<template>
  <div class="note-selectors">
    <NoteSelector active="true" placeholder="First note..." />
    <NoteSelector />
    <NoteSelector />
    <!-- <div class="note-selector active">
      <p class="note-selector-title">First note...</p>
      <p class="note-selector-timestamp">Timestamp here...</p>
    </div>
    <div class="note-selector">
      <p class="note-selector-title">Second note...</p>
      <p class="note-selector-timestamp">Timestamp here...</p>
    </div>
    <div class="note-selector">
      <p class="note-selector-title">Third note...</p>
      <p class="note-selector-timestamp">Timestamp here...</p>
    </div> -->
  </div>
</template>

<script>
import NoteSelector from "./NoteSelector";

export default {
  name: "note-selectors",
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
