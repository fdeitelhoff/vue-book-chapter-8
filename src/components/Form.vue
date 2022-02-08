<template>
  <div class="container">
    <div class="form-row">
      <div class="form-group col-md-3">
        <label for="inputEmail4">Email</label>
        <input
          type="email"
          class="form-control"
          id="inputEmail4"
          placeholder="Email"
        />
      </div>
      <div class="form-group col-md-3">
        <label for="inputEmail4">Email</label>
        <input
          type="email"
          class="form-control"
          id="inputEmail4"
          placeholder="Email"
        />
      </div>
      <div class="form-row">
      <div class="form-group col-md-6">
        <label for="inputEmail4">Email</label>
        <input
          type="email"
          class="form-control"
          id="inputEmail4"
          placeholder="Email"
        />
      </div>
    </div>

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
