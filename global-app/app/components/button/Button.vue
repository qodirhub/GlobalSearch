<template>
    <button class="mx-auto">
      <a
        class="
          custom-btn
          btn-13
          flex
          border-4
          hover:border-lime-400
          rounded-full
          bg-[#308d8a]
          w-auto
          xs:hidden
          text-white
          pl-6
          py-3
          px-4
        "
        href=""
        >
        <slot></slot>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="arrow1 w-6 h-6"
          className="h-2 w-2"
          viewBox="0 0 20 20"
          fill="currentColor"
        >
          <path
            class="mr-0"
            fillRule="evenodd"
            d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
            clipRule="evenodd"
          /></svg
      ></a>
    </button>
</template>

<script>
export default {

};
</script>

<style scoped>
* {
  font-family: 'Maven Pro', sans-serif;
  font-weight: 600;
}

/* |||||| ARROW ANIMATION |||||| */
.arrow1 {
  animation: slide1 1s ease-in-out infinite;
  margin-left: 0px;
}

@keyframes slide1 {
  0%,
  100% {
    transform: translate(0, 0);
  }

  50% {
    transform: translate(10px, 0);
  }
}
/* |||||| END ARROW ANIMATION |||||| */



/* |||||||||  BUTTON ANIMATION  ||||||||||| */
.custom-btn {
  color: #fff;
  border-radius: 5px;
  background: transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  box-shadow: inset 2px 2px 2px 0px rgba(255, 255, 255, 0.5),
    7px 7px 20px 0px rgba(0, 0, 0, 0.1), 4px 4px 5px 0px rgba(0, 0, 0, 0.1);
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
  box-shadow: -7px -7px 20px 0px #fff9, -4px -4px 5px 0px #fff9,
    7px 7px 20px 0px #0002, 4px 4px 5px 0px #0001;
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
/* ||||||||| END BUTTON ANIMATION  ||||||||||| */

</style>