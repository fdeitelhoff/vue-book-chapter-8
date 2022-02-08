<template>
  <div>
    <input v-model="name" placeholder="Veranstaltungsname…" />
    <br />
    <textarea
      v-model="information"
      placeholder="Informationen zur Veranstaltung…"
    ></textarea>
    <br />
    <input type="checkbox" v-model="isOnlineEvent" />
    <br />
    <input type="radio" v-model="isEventSeries" />
    <br />
    <select v-model="eventLocation">
      …
    </select>
  </div>
</template>

<script>
export default {
  name: 'Form',
  data: () => {
    return {
      name: '',
      information: '',
      isOnlineEvent: true,
      isEventSeries: false,
      eventLocation: '',
    };
  },
};
</script>
