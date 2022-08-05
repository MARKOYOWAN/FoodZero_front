<template>
  <div class="master">
    <div class="row primary">
      <div class="column about">
        <h3 id="name">FoodZero</h3>  
      </div>

  

      <div class="column links">
        <h3>Contact</h3>
        <ul>
          <li>
               <div class="_contact">
                <a href="#faq">+1+86852 346 000</a>
                <a href="#faq">info@test.com</a>
            </div>
          </li>
          <li>
               <div class="_contact">
                <a href="#faq">1959 Sepulveda Blcd</a>
                <a href="#faq">Culver City,CA, 90230 </a>
            </div>
          </li> 
        </ul>
      </div>

      <div class="column subscribe">
        <h3>Never Miss a Recipe</h3>
           <div class="email_button" >
          <input type="email" placeholder="Your email id here" />
          <button>Subscribe</button>
        </div>
      </div>
    </div>
 
  </div>
</template>

<script>
export default {
  name: "FooterPage",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
.master {
    background-color: #233000;
}

._contact {
    display: flex;
    flex-direction: column;
}
#name {
    padding-top: 30px;
    font-size: 40px;
}
body {
  padding: 0;
  margin: 0;
  min-height: 100vh;
  display: flex;
  align-items: flex-end;
}
footer {
  background-color: #121315; 
  font-size: 16px;
}
footer * {
  font-family: "Poppins", sans-serif;
  box-sizing: border-box;
  border: none;
  outline: none;
}
.row {
  padding: 1em 1em;
}
.row.primary {
  display: grid;
  grid-template-columns: 2fr 1fr  2fr;
  align-items: stretch;
}
.column {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 0 2em;
padding-top: 40px;
  min-height: 15em;
}
h3 {
  width: 100%;
  text-align: left;
  color: white;
  font-size: 1.4em;
  white-space: nowrap;
}
ul {
  list-style: none;
  display: flex;
  flex-direction: column;
  padding: 0;
  margin: 0;
}
li:not(:first-child) {
  margin-top: 0.8em;
}
ul li a {
  color: white;
  text-decoration: none;
}
ul li a:hover {
  color:  black;
}
.about p {
  text-align: justify;
  line-height: 2;
  margin: 0;
}
input { 
  padding: 1em; 
  border-radius: 5px;
  margin-bottom: 5px;
  background-color: #233000; 
  border-color: white;
  width: 500px;
}

 input::placeholder{
  color: white;
}
button {
  background-color:  #5E6600;  
    border-color : #5E6600;
    color: white;
      padding: 1em; 
        border-radius: 5px;
        width: 20%;
}

.email_button {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
} 
div.social {
  display: flex;
  justify-content: space-around;
  font-size: 2.4em;
  flex-direction: row;
  margin-top: 0.5em;
}
.social i { 
}

.copyright {
  padding: 0.3em 1em;
  background-color: #25262e;
}
.footer-menu {
  float: left;
  margin-top: 10px;
}

.footer-menu a {
  color: #cfd2d6;
  padding: 6px;

  text-decoration: none;
}
.footer-menu a:hover {
  color: #27bcda;
}
.copyright p {
  font-size: 0.9em;
  text-align: right;
}
@media screen and (max-width: 850px) {
  .row.primary {
    grid-template-columns: 1fr;
  }
}

@media (max-width:500px) {
.footer-menu ul{
  display: flex;
  margin-top: 10px;
  margin-bottom: 20px;
}
}
</style>
