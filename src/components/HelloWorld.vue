<template>
    <div>
        <input type="text" v-model="message" placeholder="edit me" ref="count">
        <div>{{counters}}</div>

    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
      return {
          counters:0
      };
      count : this.$refs.count.value;
  },
    methods:{
      add(){
          this.counter++;
      },
        sub(){

          {this.counter--;}
        }
    }

}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
