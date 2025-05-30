<script setup></script>
<template>
  <main class="bg--home irl flex-col justify-center text-center shadow-lg">
    <h3
      class="text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-blue-500 mb-3 font-extrabold text-7xl welcome"
    >
      Welcome to
    </h3>
    <h1
      class="text-transparent bg-clip-text bg-gradient-to-r from-red-400 to-blue-500 mb-3 font-extrabold text-8xl pb-2 name"
    >
      Programmatic
    </h1>
    <router-link to="/enroll"
      ><button
        class="bg-gray-600 hover:bg-gray-500 active:bg-gray-600 p-3 rounded shadow-md font-bold text-blue-300 m-8"
        role="link"
      >
        Get Started &rarr;
      </button></router-link
    >
  </main>
  <hr class="mx-auto w-5/6 mb-24 border border-slate-400 mt-10" />
  <article class="flex-col flex justify-center items-center">
    <h2 class="text-8xl font-extrabold text-center text-white mt-5 mb-3 offer">
      Who Are We?
    </h2>
    <hr class="mx-auto w-1/4 mb-20 border border-purple-700" />
    <section class="flex flex-col justify-center gap-36">
      <div class="flex justify-center">
        <div class="flex justify-center flex-col">
          <p
            class="txt-custom-scr mt-2 mb-4 text-lg text-gray-300 justify-center text-center"
          >
            Programmatic is a nonprofit under Hackclub that helps kids learn coding and hardware by working on real projects. We guide them through building websites, creating games, wiring circuits, and designing tech solutions. By making tech hands-on and fun, we give students the tools to solve problems and gain confidence in their abilities. Our focus is on giving kids practical skills they can use in the real world.
          </p>
          <a
            href="#/about"
            class="text-blue-300 transition hover:text-purple-300 duration-500 text-xl text-center justify-center"
            >About →</a
          >
        </div>
      </div>
    </section>
  </article>
  <hr class="mx-auto w-5/6 mb-24 border border-slate-400 mt-32" />
  <article class="flex-col flex justify-center items-center">
    <h2 class="text-8xl font-extrabold text-center text-white mt-24 mb-3 offer">
      What Can We Offer?
    </h2>
    <hr class="mx-auto w-1/3 mb-24 border border-purple-700 mt-1" />
    <section class="flex flex-col justify-center gap-36">
      <div class="flex justify-center gap-24 items-center z-flex">
        <div class="image-container">
          <img class="w-custom-scr rounded" src="../assets/circuit.avif" alt="" />
        </div>
        <div>
          <h2
            class="txt-custom txt-title text-5xl font-extrabold py-5 text-white mt-1"
          >
          Coding, Hardware, and Problem Solving
          </h2>
          <p class="txt-custom mt-4 py-1 mb-4 text-lg text-gray-300">
            In our classes, students will learn to build websites, program games, design circuits, and create their own tech solutions. Beyond technical skills, they'll develop creativity, critical thinking, and confidence as they tackle challenges and bring their ideas to life. Our goal is to provide a learning environment that encourages exploration, builds practical skills, and helps kids gain a deeper understanding of how technology works in the world around them.
          </p>
          <router-link
            to="/enroll"
            class="text-blue-300 transition hover:text-purple-300 duration-500 text-xl"
            >Enroll →</router-link
          >
        </div>
      </div>

      <!--  -->
      <!--  -->
      <!--  -->

      <div class="flex justify-center gap-24 items-center z-flex z-flip">
        <div>
          <h2
            class="txt-custom txt-title text-5xl font-extrabold py-5 text-white mt-1"
          >
            Volunteer
          </h2>
          <p class="txt-custom mt-4 mb-4 py-1 text-lg text-gray-300">
            Want to help? Programmatic is the perfect place for programmers and developers interested in teaching STEM. Not only will you gain experience improving your presentation and teaching skills, but you can also earn volunteer hours while helping the next generation of students learn computer science. Choose from five courses to teach or contribute to expanding and developing Programmatic.
          </p>
          <a
            href="#/volunteer"
            class="text-blue-300 transition hover:text-purple-300 duration-500 text-xl"
            >Volunteer →</a
          >
        </div>
        <div class="image-container">
          <img class="w-custom-scr rounded" src="../assets/car.png" alt="" />
        </div>
      </div>
    </section>
  </article>
  <hr class="mx-auto w-5/6 mb-24 border border-slate-400 mt-32" />
  <section class="flex flex-col justify-center mb-10 items-center">
    <h4 class="text-center text-5xl font-extrabold text-white mt-1 mb-10">
      Contact Us
    </h4>
    <p class="text-center text-2xl text-white m-5 contact">
      Got questions? Reach out to us! We're here to answer your inquiries,
      provide more information about our programming classes and volunteering
      opportunities, and guide you through the exciting journey ahead.
    </p>
    <h5 class="text-2xl text-center text-white font-bold p-2 gmail">
      programmaticteams@gmail.com
    </h5>
  </section>
</template>

<style scoped>
.contact {
  width: 1200px;
  max-width: 1200px;
  margin-top: 0;
}
.w-custom-scr {
  width: 500px;
}
.txt-custom-scr {
  width: 880px;
}

.bg--home {
  background-image: url("https://images.unsplash.com/photo-1625535163131-9d1fc30ea5f5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2664&q=80");
  background-repeat: no-repeat;
  width: calc(100vw - (100vw - 100%));
}

.image-container {
  display: inline-block;
  position: relative;
  /* Required for positioning the light effect */
}

.image-container img {
  border: 10px transparent;

  box-shadow: 0 0 20px rgba(131, 1, 131, 0.7);

  transition: box-shadow 0.75s ease-in-out;
}

.image-container:hover img {
  box-shadow: 0 0 30px rgb(100, 0, 128);
}

@media (max-width: 1630px) {
  .txt-custom {
    width: 500px;
  }
}

@media (max-width: 1250px) {
  .w-custom-scr {
    width: 400px;
  }

  .contact {
    width: 800px;
  }
}

@media (max-width: 1100px) {
  .txt-custom {
    width: 400px;
  }

  .contact {
    width: 600px;
  }

  .z-flex {
    flex-direction: column;
    gap: 1rem;
    text-align: center;
  }

  .z-flip {
    flex-direction: column-reverse;
  }

  .txt-title {
    padding-bottom: 0.1rem;
  }

  .txt-custom-scr {
    width: 680px;
  }
}

@media (max-width: 800px) {
  .name {
    font-size: 4rem;
  }

  .welcome {
    font-size: 2.5rem;
  }

  .txt-custom-scr {
    width: 450px;
  }

  .contact {
    width: 400px;
  }

  .name {
    font-size: 3.5rem;
  }

  .offer {
    font-size: 4rem;
  }

  .gmail {
    font-size: 1rem;
  }
}

@media (max-width: 500px) {
  .w-custom-scr {
    width: 300px;
  }
  .txt-custom {
    width: 300px;
  }
  .name {
    font-size: 3rem;
  }

  .welcome {
    font-size: 2rem;
  }

  .txt-custom-scr {
    width: 300px;
  }

  .contact {
    width: 300px;
  }

  .name {
    font-size: 2.5rem;
  }
}
</style>
