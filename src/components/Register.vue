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
            you are a beginner or an aspiring pro-cyclist!
          </p>
        </div>
      </div>
    </div>
  </div>  
</section>
      
      <div class="col-sm-5">
        <div class="form-data">

        </div>
        <div class="form-body">
          <div class="row form-row">

          </div>
        </div>
      </div>


<div class="col-lg-6 col-md-6 col-sm-12">
<form @submit.prevent="handleSubmit">
          <label class="h4 text-dark">Let's Get Started:</label>
              <h1 class="sign">Register:</h1>
    <br /><br />
    <label>Email</label>
    <input type="email" required v-model="email">

    <label>Password</label>
    <input type="password" required v-model="password">
    <div v-if="passwordError" class="error">{{ passwordError }}</div>

<label>Role:</label>
<select v-model="role">
<option value="Aspiring Pro Cyclist">Aspiring Pro Cyclist</option>
<option value="Elite Cyclist">Elite Cyclist</option>
</select>

<div class="terms">
  <input type="checkbox" v-model="terms" required />
  <label>Accept terms and conditions</label>
</div>
  <div class="submit">
    <button>Register</button>
  </div>
</form>
</div>

<p>Email: {{ email }}</p>
<p>Password: {{ password }}</p>
<p>Role: {{ role }}</p>
<p>Terms accepted: {{ terms }}</p>
</template>

<script>
export default {
  data() {
    return {
      email: "Al",
      password: "",
      role: "Aspiring Pro Cyclist",
      terms: false
    };
  },
  methods: {
    addRole(e) {
      if (e.key === "," && this.tempRole) {
        if (!this.Role.includes(this.tempRole)) {
          this.Role.push(this.Role)
        }
        this.Role = ""
      }
    },
    deleteRole(role) {
      this.Role = this.Role.filter((item) => {
        return role !== item
      })
    },
    handleSubmit() {
      //validate pwd
      this.passwordError =
        this.password.length > 5 ?
          "" : "Password must be at least 6 characters long."
      if (!this.password) {
        console.log("email: ", this.email);
        console.log("password: ", this.password);
        console.log("role: ", this.role);
        console.log("terms accepted: ", this.terms);
      }
    }
  }
}
 
    // handleSubmit() {
    //   fetch("https://booking--system-coach-client.herokuapp.com/contact", {
    //     method: "POST",
    //     body: JSON.stringify({
    //       name: this.name,
    //       email: this.email,
    //       message: this.message,
    //     }),
    //     headers: {
    //       "Content-type": "application/json; charset=UTF-8",
    //     },
    //   })
    //     .then((res) => res.json())
    //     .then((data) => (this.contact = data))
    //     .catch((err) => console.log(err.message));
    // }

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


 .content {
   margin-top: 15%;
   text-align: center;
   color: #FFF;
 /* padding: 30px; */
 }
.content h1{
  font-weight: 600;
  font-size: 3.5rem;
}
@media screen and (max-width: 967px){

}

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
.submit {
  /* border: ; */
  color: white;
  border-radius: 20px;
    text-align: center;

}

.error {
  color: #ff0062;
  margin-top: 10px;
  font-size: 0.9em;
  font-weight: bold;
}

.register {
  text-align: center;
}
</style>