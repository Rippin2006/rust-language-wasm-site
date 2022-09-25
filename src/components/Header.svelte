<script>
  import logo from '../assets/SSR1234.png';
  let test12 = 'We are SSR';
</script>

<div class="header">
  <img class="logo" src={logo} alt="logo" >
  <p>{test12} </p>
</div>

<style>
  .header {
  padding: 50px;
  text-align: center;
  height: calc(100vh - 200px);
  background-image: linear-gradient(0deg, #000000, #000000, #000000);
}
.logo {
  height: 70%;
}
p {
  font-size: calc(max(1.5vw, 55px));
  color: #dfeeed;
}
@media screen and (max-width: 500px) {
    .logo {
      height: 30%;
    }
  }
  @media screen and (max-width: 300px) {
    .logo {
      height: 25%;
    }
  }
  @media screen and (max-width: 400px) {
    .logo {
      height: 20%;
      min-height: 15%;
    }
  }
</style>