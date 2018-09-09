<template>
  <div class="container">
    <form>
      <div class="form-group">
        <label for="comment-title">Title</label>
        <input type="text" class="form-control" id="comment-title" v-model="comment.title">
      </div>
      <div class="form-group">
        <label for="comment-details">Message</label>
        <textarea rows="15" class="form-control" id="comment-details" v-model="comment.details"></textarea>
      </div>
      <button class="btn btn-primary" @click.prevent="onSubmit">Submit</button>
    </form>
    <br/>

  </div>
</template>
<script>
export default {
  data() {
    return {
      comment: {
        title: "",
        details: ""
      }
    };
  },
  created() {},
  methods: {
    onSubmit() {
      console.log(this.comment.title);
    }
  }
};
</script>
