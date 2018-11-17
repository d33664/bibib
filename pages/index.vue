<template>
  <div class="flex-container">
    <div class="text-wrap">
      <div class="text-item">
        <h2>Lorem, ipsum.</h2>
      </div>
      <div class="text-item">
        <h1>Lorem ipsum dolor sit</h1>
      </div>
    </div>
    <div class=main-Img>
      <img src="https://picsum.photos/900/700" width="900" height="700" alt=""></div>
  </div>
</template>

<style>
.main-img {
  width: 80%;
  margin-top: 20px;
}
.text-wrep{
  width: 20%;
  position: relative;
}

.text-wrap .text-item {
  position: absolute;
  left: 180px;
  top: 150px;
}

.text-wrap .text-item:nth-child(1){
  width: 100px;
}

.text-wrap .text-item:nth-child(2) {
  top: 330px;
  width: 70px;
}

  .text-wrap .text-item h1 {
  background: #ffffff;
  padding: 3px;
  text-transform: uppercase;
  display: inline;
  font-size: 70px;
  letter-spacing: 11px;

  }
  @media only screen and (max-width: 480px){
    .text-wrap .text-item:nth-child(1) h2{
      background-color: #ffffff;
      display: inline;
      letter-spacing: 8px;
    }
    .text-wrap{
      width: 0;
    }
  }

</style>
