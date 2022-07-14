<template>
  <header class="w-full scroll-m-2 2xl:sticky xl:sticky lg:static top-0 z-50 bg-[#c8ece1]" :class="{ 'scrolled': !view.atTopOfPage }" >

    <div class="container mx-auto px-40 xs:px-5">
      <nav class="flex justify-between">
        <div class="flex justify-between">
          <a href="#"><img class="w-20 xs:w-15" src="/img/my-logoo.png" alt=""></a>
        </div>
        <div class="mx-auto xs:mx-0 xs:ml-auto">
          <ul class="flex py-6 md:space-x-10 text-base xs:text-xs text-center">
            <li class="text-center"><a class="py-2 px-3 text-center hover:text-white hover:bg-[#308d8a] transition duration-300 ease-out hover:ease-in" href="#">Home</a></li>
            <li class="text-center"><a class="py-2 px-3 text-center hover:text-white hover:bg-[#308d8a] transition duration-300 ease-out hover:ease-in" href="#">About Us</a></li>
            <li class="text-center"><a class="py-2 px-3 text-center hover:text-white hover:bg-[#308d8a] transition duration-300 ease-out hover:ease-in" href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="flex">
          <my-button>
            Go App
          </my-button>
        </div>

      </nav>
    </div>

  </header>
</template>

<script>
import myButton from '/components/button/Button.vue'
export default {
  components: {
    "my-button": myButton
  },
  data () {
    return {
        view: {
            atTopOfPage: true
        }
    }
},

// a beforeMount call to add a listener to the window
beforeMount () {
    window.addEventListener('scroll', this.handleScroll);
},

methods: {
	// the function to call when the user scrolls, added as a method
    handleScroll(){
        // when the user scrolls, check the pageYOffset
        if(window.pageYOffset>0){
            // user is scrolled
            if(this.view.atTopOfPage) this.view.atTopOfPage = false
        }else{
            // user is at top of page
            if(!this.view.atTopOfPage) this.view.atTopOfPage = true
        }
    }
}
}
</script>

<style scoped>
* {
  font-family: 'Maven Pro', sans-serif;
  font-weight: 600;
}



/* |||||||||  HEADER SCROLL SHADOW  ||||||||||| */

header.scrolled {
    @apply shadow-2xl;
    border-bottom: 0px;
}

/* |||||||||  END HEADER SCROLL SHADOW  ||||||||||| */
</style>
