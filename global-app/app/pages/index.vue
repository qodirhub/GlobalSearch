<template>
  <div>
    <Header />

    <div class="w-full relative z-40 bg-[#c8ece1]">
      <div class="">
        <div class="grid grid-cols-2 xs:grid-cols-1 xs:flex xs:flex-col-reverse px-40 xs:px-5">
          <div class="my-28 xs:my-5 flex items-center xs:flex xs:items-center xs:justify-center">
            <div class="justify-center xs:text-center">
              <h2 class="font-extrabold text-6xl xs:text-4xl mb-4 text-[#308d8a]">Simple Solution</h2>
              <h2 class="text-5xl font-bold mb-4  xs:text-2xl">we take a simple <br> approach  to solutions</h2>
              <p class=" mb-4">Receive mSOL, the ultimate unit of <br> the Solana ecosystem.</p>
              <my-button>
                Read more..
              </my-button>
              <!-- <button class="custom-btn btn-13 transition ease-in-out delay-150  hover:-translate-y-1 rounded-full bg-[#308d8a] w-auto text-white font-bold">Read more..</button> -->
            </div>
          </div>
          <div class="my-28 xs:my-10 xs:flex xs:items-center xs:justify-center">
            <img
              class="2xl:ml-3 xs:ml-5 absolute 2xl:fixed z-1 md:w-32 lg:w-full"
              src="/img/white-clouds.svg"
              alt=""
            />
            <img
              class="w-96 xs:w-60  2xl:ml-auto relative z-2"
              src="/img/Coding_SVG.svg"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
    
    <Footer />

    <Iconcode />
  </div>
</template>

<script>
import myButton from '/components/button/Button.vue'
export default {
    components: {
    "my-button": myButton
  },
}
</script>

<style scoped>

/* ||||||||||||||| BUTTON ANIMATION  ||||||||||||||||| */
.custom-btn {
  width: 130px;
  height: 40px;
  color: #fff;
  border-radius: 5px;
  background: transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  display: inline-block;
   box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
   7px 7px 20px 0px rgba(0,0,0,.1),
   4px 4px 5px 0px rgba(0,0,0,.1);
  outline: none;
}
.btn-13 {
  background-color: #308d8a;
background-image: linear-gradient(315deg, #308d8a 0%, #308d8a 74%);
  border: none;
  z-index: 1;
}
.btn-13:after {
  position: absolute;
  content: "";
  width: 100%;
  height: 0;
  bottom: 0;
  left: 0;
  z-index: -1;
  border-radius: 5px;
   background-color: #4dccc6;
background-image: linear-gradient(315deg, #4dccc6 0%, #96e4df 74%);
  box-shadow:
   -7px -7px 20px 0px #fff9,
   -4px -4px 5px 0px #fff9,
   7px 7px 20px 0px #0002,
   4px 4px 5px 0px #0001;
  transition: all 0.3s ease;
}
.btn-13:hover {
  color: #fff;
}
.btn-13:hover:after {
  top: 0;
  height: 100%;
}
.btn-13:active {
  top: 2px;
}
/* ||||||||||||||| END BUTTON ANIMATION  ||||||||||||||||| */

</style>
