<template> 
  <body>
    <div class="hero">
    <h1></h1>
    <div class="social-links">
 <a href=""><i class="bi bi-facebook"></i></a>
 <a href=""><i class="bi bi-twitter"></i></a>
 <a href=""><i class="bi bi-linkedin"></i></a>
 <a href=""><i class="bi bi-youtube"></i></a>
 <a href=""><i class="bi bi-instagram"></i></a>
    </div>
  </div>
  </body>
</template>

<script>
</script>


<style>
*{
  padding: 0;
  margin:0;
  font-family: 'Times New Roman', Times, serif;
}
.hero{
  width:100%;
  height: 100vh;
  background: #d2dde4;
  display: flex;
  align-items:center;
  flex-direction: coloumn;
  justify-content: center;
}
h1{
  font-size: 40px;
  margin-bottom: 100px;
  margin-top: -100px;
  margin-left: -1pc;
}
.social-links{
  display: flex;
}
.social-links a{
  width:80px;
  height:80px;
  text-align: center;
  text-decoration: none;
  color: #8b2929;
  box-shadow: 0 0 20px 10px rgba(5, 44, 2, 0.05);
  margin: 0 30px;
  border-radius: 50%;
  position: relative;
  overflow: hidden;
  transition: transform 0.5s;
}
.social-links a .bi{
  font-size: 30px;
  line-height: 80px;
  position: relative;
  z-index: 10;
  transition: color 0.5s;
}
.social-links a::after{
  content: '';
  width: 100%;
  height: 100%;
  top:-90px;
  left: 0;
  background: linear-gradient(-45deg, #ed1c94, #ffec17);
  position: absolute;
  transition: 0.5s;
}
.social-links a:hover::after{
top:0;
}
.social-links a:hover .bi{
  color: #fff;

}
.social-links a:hover{
  transform: translateY(-10px);
}
</style>