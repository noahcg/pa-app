<template>
  <div class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-white border-bottom shadow-sm">
    <h5 class="my-0 mr-md-auto font-weight-normal">{{ personal.firstName }} {{ personal.lastName }}</h5>
    <div class="my-2 my-md-0 mr-md-3 text-right">
      <p>{{ displayDate(new Date()) }}<br />
        <small>{{ displayTime() }}</small>
      </p>
    </div>
</div>
</template>

<script>
import moment from 'moment';

export default {
  name: 'Header',
  props: {
    msg: String,
    personal: {
      firstName: {
        type: String,
        required: false,
      },
      lastName: {
        type: String,
        required: false,
      },
      age: {
        type: Number,
        required: false,
      },
    },
  },
  methods: {
    displayDate(date) {
      return moment(date).format('dddd, MMMM D, YYYY');
    },
    displayTime() {
      return moment(new Date()).format('h:mm a');
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
