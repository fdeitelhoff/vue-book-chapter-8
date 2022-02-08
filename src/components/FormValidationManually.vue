<template>
  <div>
    <form
      @submit="validateForm">
    <p v-if="errors.length">
      <span>Bitte prüfen Sie Ihre Eingabe!</span>
      <ul>  
        <li v-for="error in errors">{{ error }}</li>
      </ul>
    </p>
  <p>
    <input v-model="name" placeholder="Veranstaltungsname…" />
    </p>
    <p>
    <textarea
      v-model="information"
      placeholder="Informationen zur Veranstaltung…"
    ></textarea>
    </p>
    <p><input type="checkbox" v-model="isOnlineEvent" />
    </p>
    <p>
    <input type="radio" v-model="isEventSeries" />
    </p>
    <p>
    <select v-model="eventLocation">
      …
    </select>
    </p>
      <p>
    <input
      type="submit"
      value="Submit"
    >
  </p> 
    </form>
  </div>
</template>

<script>
export default {
  name: 'FormValidationManually',
  data: () => {
    return {
      errors: [],
      name: '',        
      information: '',
      isOnlineEvent: true,
      isEventSeries: false,
      eventLocation: '',
    };
  },
  methods: {
    validateForm(e) {
      console.log('validate form:', e);

      if (!this.name) {
        this.errors.push("Der Name ist verpflichtend!");
      }
    }
  }
};
</script>
