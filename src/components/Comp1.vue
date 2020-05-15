<template>
  <div>
    <h1>{{ heading }}</h1>
    <button @click="incr" class="btn">Incr count++</button>
    <p>Count is: {{ count }}</p>
    <p>Prop1 is: {{ prop1 }}</p>
  </div>
</template>
<script>
export default {
  name: "Comp1",
  props: {
    prop1: String
  },
  data: function() {
    return {
      heading: "This is Comp1",
      count: 0
    };
  },
  methods: {
    incr: function() {
      this.count += 1;
      this.$emit("custom-event", "Some message");
    }
  }
};
</script>
<style scoped>
.btn {
  background-color: red;
  color: white;
}
</style>
