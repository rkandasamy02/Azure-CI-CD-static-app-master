<template>
  <div class="hello">
    <div>
      <form>
        <label for="name">Name:</label>
        <input type="text" v-model="name" id="name" name="name" required />
        <br />
        <br />
        <label for="email">Email:</label>
        <input type="email" v-model="email" id="email" name="email" required />
        <br />
        <br />
        <label for="phone">Phone:</label>
        <input type="tel" v-model="phone" id="phone" name="phone" required />
        <br />
        <br />
        <label for="file-upload">Upload File:</label>
        <input type="file" id="file-upload" ref="file" @change="uploadFile" />
        <br />
        <br />
        <button type="submit" @click="submitForm">Submit</button>
        <br />
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      name: "",
      email: "",
      phone: "",
      file: "",
    };
  },
  methods: {
    submitForm() {},
    uploadFile(e) {
      this.file = e.target.files[0];
      // handle the file here
    },
  },
};
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
