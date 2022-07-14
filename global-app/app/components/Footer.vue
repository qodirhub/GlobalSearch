<template>
    <div class="w-full h-full relative overflow-x-hidden flex items-center justify-around z-40 md:w-auto">
      <div class="px-40 xs:px-5">
          <h1 class="flex justify-center items-center mt-8 font-bold text-6xl mb-4 text-[#308d8a] text-shadow-sm xs:text-4xl">Why us?</h1>
        <div class="w-full flex justify-end">
          <div class="absolute bg-[#308d8a] w-64 h-64 -mt-24 rounded-full mix-blend-multiply filter blur-xl animate-blob animation-delay-2000 opacity-70"></div>
        </div>
        <div class="flex grid-cols-2 gap-2 xs:flex-none xs:gap-1 xs:grid-cols-1">
          <div class="col-span-2 max-w-2xl xs:col-span-1 my-28 xs:my-3 flex items-center relative">
            <div class="md:w-auto">
              <h2 class=""></h2>
              <h2 class="font-extrabold text-6xl mb-4 text-[#308d8a]">Simple Solution</h2>
              <ul class="list-disc list-inside my-3">
                <li class="text-[#308d8a] font-bold text-lg">Everything is easy and simple for us.</li>
                <li class="text-[#308d8a] font-bold text-lg">Fast and high quality.</li>
                <li class="text-[#308d8a] font-bold text-lg">We have experienced programmers.</li>
                <li class="text-[#308d8a] font-bold text-lg">We have a great team.</li>
              </ul>
              <p class="mr-10 xs:m-0 mb-4 xs:w-full"> <span class="text-[#308d8a] font-bold text-lg">Simple Solution</span>  - provides a wide range of services in the field of IT. 
                We mainly develop high load backend systems and more. Our services are used by 
                banks, payment systems, suppliers of self-service terminals and those who need 
                to qualitatively serve a large number of customers. We develop multi-modular 
                projects for convenience in addition and expansion in the future. Always ready 
                to discuss client problems and give a right solution to the business.
              </p>
              <!-- <button class="custom-btn btn-13 transition ease-in-out delay-150  hover:-translate-y-1 rounded-full bg-[#308d8a] w-auto text-white font-bold">Read more..</button> -->
            </div>
          </div>

          <div class="mb-20 xs:my-3">
            <div class="flex">
            <img
              class="w-screen relative"
              src="/img/team-our.svg"
              alt=""
            />
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<style scoped>

 /* ||||||||| TITLE |||||||||| */
.white-shadow {
  /* font-size:120px; */
	letter-spacing:0.1em;
  -webkit-text-fill-color: transparent;
  /* -webkit-text-stroke-width: 2px; */
  /* -webkit-text-stroke-color: white; */
  text-shadow: 
						1px 1px #308d8a,
						3px 3px #fff;
}
 /* ||||||||| END TITLE |||||||||| */



 /* ||||||||| BUTTON STYTLE |||||||||| */
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
 /* ||||||||| END BUTTON STYTLE |||||||||| */

</style>
