<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>

/* navbar */
body {
    margin:0;
    padding:0;
    background:#262626;
    background-image:url(/background.jpg);
    background-size:cover;
    background-attachment: fixed;
}
.buttons {
    margin:0;
    padding:0;
    position:absolute;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    background:red;
}
.buttons li {
    display:inline-block;
    transform-style:preserve-3d;
}
.buttons li a {
    color:#262626;
    font-size:16px;
    font-familY:arial;
    text-transform: uppercase;
    text-decoration:none;
    font-weight:bold;
    display:block;
    position:relative;
}
.buttons li a span {
    display:block;
    padding:15px 20px;
}
.buttons li a span:before {
    content:attr(title);
    position:absolute;
    top:0;
    left:0;
    background:#f30000;
    color: black;
    padding:15px 20px;
    transform-style:preserve-3d;
    transition:.3s;
    transform:rotateX(90deg) translateY(50px);
    transform-origin:bottom;
}
.buttons li a span:hover:before {
    transform:rotateX(0deg) translateY(0px);
}
.buttons li a span:after {
    content:attr(title);
    position:absolute;
    top:0;
    left:0;
    background: black;
    color:red;
    padding:15px 20px;
    transform-style:preserve-3d;
    transition:.3s;
    transform:rotateX(0deg) translateY(0px);
    transform-origin:top;
}
.buttons li a span:hover:after {
    transform:rotateX(90deg) translateY(-10px);
}
.navbar{
  top: 30px
}
.listRoom{
    font-family: 'Orbitron', sans-serif;
    text-shadow: 4px 4px 4px #aaa;
    font-size: 20px;
}





</style>
