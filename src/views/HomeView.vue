<template>
  <main
    class="mt-10 md:mt-1 flex flex-col-reverse gap-8 items-center md:flex-row md:gap-16 md:justify-center min-h-[65vh] md:min-h-[80vh]">
    <div class="space-y-2 text-center md:text-left px-10">
      <p class="text-amber-200">Hello World, I'm</p>
      <h1 class="text-4xl font-bold md:text-5xl text-white fadein-up">Ihab Elrayah</h1>
      <div class="py-2">
        <h1
          class="typewrite text-xl font-semibold text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-yellow-500 md:text-2xl fadein-up"
          ref="typewriter">
          <span class="wrap">{{ txt }}</span>
        </h1>
      </div>
      <p class="text-white pr-4 fade-in-from-left">Welcome to My personal portfolio website. <span class="wave">👋🏼</span></p>
      <br>
      <!-- <button
        class="fadein-bot fade-500 flex items-center py-2 px-4 mx-auto text-sm font-medium rounded-lg border transition duration-300 md:py-2.5 md:px-5 md:mx-0 text-amber-200 border-amber-200 hover:bg-amber-200 hover:bg-opacity-10 bg-transparent focus:outline-none w-fit"><svg
          xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="mr-2 w-4 h-4">
          <path fill-rule="evenodd"
            d="M5.625 1.5H9a3.75 3.75 0 013.75 3.75v1.875c0 1.036.84 1.875 1.875 1.875H16.5a3.75 3.75 0 013.75 3.75v7.875c0 1.035-.84 1.875-1.875 1.875H5.625a1.875 1.875 0 01-1.875-1.875V3.375c0-1.036.84-1.875 1.875-1.875zm5.845 17.03a.75.75 0 001.06 0l3-3a.75.75 0 10-1.06-1.06l-1.72 1.72V12a.75.75 0 00-1.5 0v4.19l-1.72-1.72a.75.75 0 00-1.06 1.06l3 3z"
            clip-rule="evenodd"></path>
          <path
            d="M14.25 5.25a5.23 5.23 0 00-1.279-3.434 9.768 9.768 0 016.963 6.963A5.23 5.23 0 0016.5 7.5h-1.875a.375.375 0 01-.375-.375V5.25z">
          </path>
        </svg>Download Resume</button> -->
    </div>
    <div class="flex justify-center md:justify-start fadein-right"><img alt="avatar" fetchpriority="high" width="300" height="300" decoding="async" data-nimg="1"
        class="w-10/12 md:h-auto rounded-full border-4 border-amber-200 pict" src="data:image/jpeg;base64,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">
    </div>
  </main>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      toRotate: ["Software Engineer", "Software Developer",],
      period: 2000,
      txt: '',
      loopNum: 0,
      isDeleting: false,
    };
  },
  mounted() {
    this.$nextTick(() => {
      this.tick();
    });
  },
  methods: {
    tick() {
      let typewriter = this.$refs.typewriter;

      if (!typewriter) {
        return;
      }

      let i = this.loopNum % this.toRotate.length;
      let fullTxt = this.toRotate[i];

      this.txt = this.isDeleting ? fullTxt.substring(0, this.txt.length - 1) : fullTxt.substring(0, this.txt.length + 1);
      typewriter.innerHTML = `<span class="wrap">${this.txt}</span>`;

      let that = this;
      let delta = 200 - Math.random() * 100;

      if (this.isDeleting) {
        delta /= 2;
      }

      if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
      } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
      }

      setTimeout(() => {
        that.tick();
      }, delta);
    },
  }
}
</script>

<style>
body {
  overflow-y: scroll;
  overflow-x: hidden;
}

.typewrite>.wrap {
  border-right: 0.08em solid #fff;
}

.wave {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block
}

@keyframes wave-animation {
  0% {
    transform: rotate(0deg)
  }

  10% {
    transform: rotate(14deg)
  }

  20% {
    transform: rotate(-8deg)
  }

  30% {
    transform: rotate(14deg)
  }

  40% {
    transform: rotate(-4deg)
  }

  50% {
    transform: rotate(10deg)
  }

  60% {
    transform: rotate(0deg)
  }

  to {
    transform: rotate(0deg)
  }
}

.pict {
  box-shadow: 0px 0px 73px -9px rgba(255,219,112,0.44);
-webkit-box-shadow: 0px 0px 73px -9px rgba(255,219,112,0.44);
-moz-box-shadow: 0px 0px 73px -9px rgba(255,219,112,0.44);
}

.fadein-up {
  opacity: 0;
  animation-name: fadeInUp;
  animation-duration: 0.5s;
  animation-fill-mode: forwards;
  animation-delay: 500ms;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translate3d(0, 100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fade-in-from-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-right {
  opacity: 0;
  animation: fadeInRight 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInRight {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-bot {
  opacity: 0;
  animation: fadeInBot 0.5s forwards;
}

@keyframes fadeInBot {
  from {
    opacity: 0;
    transform: translate3d(0, -100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fadein-1 {
  animation-delay: 200ms;
}
.fadein-2 {
  animation-delay: 400ms;
}
.fadein-3 {
  animation-delay: 600ms;
}
.fade-500 {
  animation-delay: 500ms;
}
</style>
