<template>
  <div>
    <div class="card-deck mb-3 text-center">
      <div class="card mb-4 shadow-sm">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">About</h4>
        </div>
        <div class="card-body">
          <p>Some about content</p>
          <router-link to="/about">
            <button type="button" class="btn btn-lg btn-block btn-primary">View</button>
          </router-link>
        </div>
      </div>
      <div class="card mb-4 shadow-sm">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Locale</h4>
        </div>
        <div class="card-body">
          <p>Some locale content</p>
          <router-link to="/about">
            <button type="button" class="btn btn-lg btn-block btn-primary">View</button>
          </router-link>
        </div>
      </div>
      <div class="card mb-4 shadow-sm">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Github</h4>
        </div>
        <div class="card-body">
          <p>Some github content</p>
          <router-link to="/about">
            <button type="button" class="btn btn-lg btn-block btn-primary">View</button>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
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
