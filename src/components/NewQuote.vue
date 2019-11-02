<template>
  <div class="row">
    <form>
      <div class="col-sm-8 col-sm-offset-2 col-md-6 col-lg-offset-3 form-group">
        <label for="quote">Quote</label>
        <textarea class="form-control" rows="3" v-model="quote"></textarea>
      </div>
      <div class="col-sm-8 col-sm-offset-2 col-md-6 col-lg-offset-3 form-group">
        <button class="btn btn-primary" @click.prevent="createNew">Add Quote</button>
      </div>
    </form>
  </div>
</template>
<script>
export default {
  data: function(){
    return {
      quote:''
    };
  },
  methods:{
    createNew(){

    }
  }
};
</script>
<style >
</style>
