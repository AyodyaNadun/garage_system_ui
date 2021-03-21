<template>
  <div class="cotainer">
    <div class="bg-image"></div>
    <div class="panel">
        <div class="mainPanel">
            <div>
                <h1>Sign In</h1>
            </div>
            <div>
                <label>Username :</label>
            </div>
            <div>
                <input type="text" />
            </div>
            <div>
                <label>Password :</label>
            </div>
            <div>
                <input type="password" />
            </div>
            <p id="pgraph1"><a href="">Forgot your password?</a></p>
        <div class="linePanel">
            <button class="button" style="vertical-align:middle"><span>Log In </span></button>
        </div>
            <p id="pgraph2">Don't have an account?<a href="">Sign Up</a></p>
        </div>
    </div>    
  </div>
</template>

<script>
export default {
  name: 'Login',
  props: {
  }
}
</script>

<style scoped>
.cotainer {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 950px;
    background-color: black;
}

.bg-image {
  background-image: url("/assets/garage_wallpaper.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  filter: blur(6px);
  position: absolute;
  height: 100%; 
  width: 100%;
  background-position: center;
}

.panel {
    display: flex;
    width: 25%;
    height: 65%;
    /* border: 1px solid rgb(28, 28, 145); */
    border-radius: 10px;
    padding: 20px;
    background-color: rgb(228, 228, 228, 0.6);
    z-index: 0;
}

.mainPanel {
    width: 100%;
    margin: 0 10px 0 10px;
}

h1 {
  margin: 30px 0 60px 0;
  color: black;
}

.linePanel {
    display: flex;
    align-items: flex-end;
    height: 25%;
}

label {
    width: 95%;
    font-style: italic;
    font-size: 20px;
    color: #031b6d;
    font-weight: 300;
}

input {
    width: 98%;
    height: 40px;
    margin-bottom: 20px;
    border-top-style: hidden;
    border-right-style: hidden;
    border-left-style: hidden;
    border-bottom-style: solid;
    padding-top: 5px;
    font-size: 18px;
    letter-spacing: 0.5px;
    background-color: transparent;
}

/* ----button styles------ */
.button {
  display: inline-block;
  border-radius: 30px;
  background-color: #1e50f4;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 18px;
  padding: 15px;
  width: 100%;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}

.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: -6px;
  right: -20px;
  transition: 0.5s;
  font-size: 25px;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover {
    opacity: 0.7;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}

*:focus {
    outline: 0 !important;
}
/* ----button styles------ */

#pgraph1 {
  display: flex;
  justify-content: flex-end;
  margin: 0 10px 0 0;
  font-size: 16px;
}

#pgraph2 {
  display: flex;
  justify-content: center;
  margin: 10px;
  font-size: 16px;
}

a {
  text-decoration: none;
  color: #092276;
}
</style>
