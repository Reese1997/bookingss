<template>
<section class="register">
  <div class="container">
    <div class="row no-margin">
      <div class="col-lg-6 col-md-6 col-sm-12">
        <div class="content">
<h1>Book Your Time Slot Now and save your time</h1>
<p class="par">Unlock and perform at you TRUE potential.
Hands on coaching, training plans and resources to
   take your cycling to a whole new level, whether
    you are a beginner or an aspiring pro-cyclist!</p>
        </div>
      
      <div class="col-sm-5">
        <div class="form-data">

        </div>
        <div class="form-body">
          <div class="row form-row">

          </div>
        </div>
      </div>
</div>


<div class="col-lg-6 col-md-6 col-sm-12">
<form @submit.prevent="handleSubmit">
          <label class="h4 text-dark">Let's Get Started:</label>
              <h1 class="sign">Sign Up:</h1>
    <br /><br />
    <input type="First name" placeholder="First Name" /><br /><br />
    <input type="Last name" placeholder="Last Name" /><br /><br />
    <input type="E-mail" placeholder="E-mail" /><br /><br />
    <!-- <input type="Tel" placeholder="Tel" /><br /><br /> -->
    <router-link :to="{ path: '/login/' }"><button>Register</button></router-link>
    <!-- <button class="but" type="submit ">REGISTER!</button> --> -->
  </form>
</div>
</div>
</div>
</section>
</template>

<script>
export default {
  data() {
    return {
      contact: null,
      name: "",
      email: "",
      message: "",
    };
  },

  methods: {
    handleSubmit() {
      fetch("https://booking--system-coach-client.herokuapp.com/contact", {
        method: "POST",
        body: JSON.stringify({
          name: this.name,
          email: this.email,
          message: this.message,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((res) => res.json())
        .then((data) => (this.contact = data))
        .catch((err) => console.log(err.message));
    },
  },
};
</script>

<style>
.sign{
  color: white;
}
p {
    font-size: 50px;

}
.par{
  font-size: 20px;
}
.register {
  min-height: 100vh;
}
body {
 background-color: black;    
  width: 100%;
  height: 100%;
  /* background-image: url(../assets/landing.jpeg); */
}
/* .layer {
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 147, 173, 0,9);
  overflow: auto;
} */
.form-data {
  margin-top: 15%;
  background-color: #FFF;
}
.form-body {
  padding: 20px;
}
.form-head {
  padding: 10px;
  border-bottom: 1px solid #CCC;
}
.form-head h2 {
  font-size: 22px;
  font-weight: 600
}
.no-margin {
margin: 0px;
}
.form-row {
  margin-bottom: 15px;
}
.form-control{
  background-color: #AAA;
}
.form-control:hover {
box-shadow: none;
border: 3px solid #c91407
}
.content {
  margin-top: 15%;
  text-align: center;
  color: #FFF;;
  padding: 30px;
}
.content h1{
  font-weight: 600;
  font-size: 3.5rem;
}
@media screen and (max-width: 967px){

}

/* section {
  height: 100vh;
} */

form {
  height: 480px;
  max-width: 470px;
  margin: 30px auto;
  background: white;
  text-align: left;
  padding: 50px;
  border-radius: 10px;
  border-style: ridge;
  background: rgba(255, 255, 255, 0.15);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}
label {
  color: rgb(58, 55, 55);
  display: inline-block;
  margin: 25px 0 15px;
  font-size: 1 em;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
}
input,
select {
  display: block;
  /* padding: 10px 6px; */
  width: 100%;
  box-sizing: border-box;
  border: none;
  border-bottom: 1px solid rgb(77, 135, 202);
  color: rgb(197, 5, 5);
}
input{
  background: none;
}
.pill {
  display: inline block;
  margin: 20px 10px 0 0;
  padding: 6px 12px;
  background: #eee;
  border-radius: 20px;
  font-size: 15px;
  letter-spacing: 1px;
  font-weight: bold;
  color: rgb(197, 5, 5);
  cursor: pointer;
}
button {
  background: rgb(197, 5, 5);
  /* border: ; */
  padding: 20px 30px;
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
  font-size: 0.9em;
  font-weight: bold;
}

.mess {
  width: 100%;
}

.but {
  margin-left: 40%;
  padding: 15px 29px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
</style>