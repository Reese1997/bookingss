<template>
  <form @submit.prevent="handleSubmit">
      <label>Full Name:</label>
      <input type="name" required v-model="name">

      <label>Email:</label>
      <input type="email" required v-model="email">

      <label>Write me a message</label>
      <br>
      <textarea name="message" id="message" rows="5" placeholder="Write me a message" v-model="message"></textarea>


<div class="submit">
    <button type="submit">Send Message</button>
</div>

  </form>

  <p>Name: {{ name }}</p>
  <p>Email: {{ email }}</p>
  <p>Message: {{ message }}</p>

</template>

<script>
    export default {
        data() {
            return {
                name: '',
                email: '',
                message: ''
            }
        },
        methods: {
            handleSubmit() {
                console.log(this.name, this.email, this,message);
                fetch("http://localhost:8900/contact", {
                    method: "POST", 
                    body: JSON.stringify({
                        name: this.name, 
                        email: this.email, 
                        message: this.message
                    }), 
                    headers: {
                        "Content-Type": "application/json; charset=UTF-8"
                    },
                })
                .then((response) => response.json())
                .then((json) => alert(json.msg))
                .catch((e) => alert(e.msg))
                }
            }
        }

</script>

<style>
form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 30px;
  gap: 20px;
  width: 100%;
  margin-inline: auto;
  max-width: 600px;
  margin-top: 200px;
  background-color: rgb(19, 16, 16);
  color: white;
}
label {
    color: #aaa;
    display: inline-block;
    margin: 25px 0 15px;
    font-size: 0.8em;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: bold;
}
input, select {
    display: block;
    padding: 10px 6px;
    width: 100%;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    color: #555;
}
input[type="checkbox"] {
    display: inline-block;
    width: 16px;
    margin: 0 10px 0 0;
    position: relative;
    top: 2px;
}
.pill {
    display: inline-block;
    margin: 20px 10px 0 0;
    padding: 6px 12px;
    background: #eee;
    border-radius: 20px;
    font-size: 12px;
    letter-spacing: 1px;
    font-weight: bold;
    color: #777;
    cursor: pointer;
}
button {
    background: #0b6dff;
    border: 0;
    padding: 10px 20px;
    margin-top: 20px;
    color: white;
    border-radius: 20px;
}
.submit {
    text-align: center;
}
.error {
    color: #ff0062;
    margin-top: 10px;
    font-size: 0.8em;
    font-weight: bold;
}
textarea {
      resize: none;
      width: 100%;
      height: 100px;
}
</style>



