<template>
  <header class="bg-light text-center pb-5">
    <div class="container">
      <img
        width="150"
        height="123"
        src="@/assets/imgs/_kt.png"
        alt="Kvarner Tours Taxi Opatija"
        class="img-fluid mb-4"
      />
      <h1 class="display-3 reveal-text fw-bold">Taxi Opatija</h1>
      <p class="lead mx-2">Bez komplikacija. Brza i pouzdana taxi služba.</p>
      <a href="tel:098491369">
        <button
          class="btn btn-primary btn-lg link-light fw-bolder button-shadow w-75"
        >
          Pozovi prijevoz
        </button>
      </a>
    </div>
  </header>

  <section class="py-3 mb-3 rounded-bottom-3 mx-2 bg-light">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <div class="card mb-4 border-0 rounded-5">
            <div class="card-body">
              <h2
                class="card-title"
                style="
                  color: #333;
                  font-size: 1.8em;
                  text-align: center;
                  margin-bottom: 0.3em;
                "
              >
                0-24h
              </h2>
              <p
                class="card-text"
                style="color: #555; font-size: 1em; text-align: center"
              >
                Pozovite vožnju bilo kada, bio dan ili noć.
              </p>
            </div>
          </div>
        </div>
        <!-- <Transition name="dissapear">
          <div v-if="!racTime" class="col-md-12">
            <div>
              <div class="card mb-4 border-0 rounded-5">
                <div class="card-body">
                  <h2
                    class="card-title"
                    style="
                      color: #333;
                      font-size: 1.8em;
                      text-align: center;
                      margin-bottom: 0.3em;
                    "
                  >
                    Iskusni Vozači
                  </h2>
                  <p
                    class="card-text"
                    style="color: #555; font-size: 1em; text-align: center"
                  >
                    Iskusni vozači osposobljeni za vašu sigurnost.
                  </p>
                </div>
              </div>
            </div>
            <div>
              <div class="card mb-4 border-0 rounded-5">
                <div class="card-body">
                  <h2
                    class="card-title"
                    style="
                      color: #333;
                      font-size: 1.8em;
                      text-align: center;
                      margin-bottom: 0.3em;
                    "
                  >
                    Visoki Standardi
                  </h2>
                  <p
                    class="card-text"
                    style="color: #555; font-size: 1em; text-align: center"
                  >
                    Svako vozilo je podvrgnuto detaljnom čišćenju i redovitom
                    održavanju radi vaše sigurnosti i udobnosti.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </Transition> -->
      </div>
    </div>
  </section>

  <Transition name="slide-fade" appear>
    <section
      class="py-3 mx-2 mx-1 rounded-5 rounded-bottom-0 shadow-lg bg-white"
      v-if="racTime"
    >
      <div class="container">
        <img
          width="200"
          height="165"
          src="@/assets/imgs/_kt.png"
          alt="Rent a Car & Van Kvarner Tours"
          class="img-fluid mb-4"
          loading="lazy"
        />
        <h3 class="fs-1 reveal-text fw-bold">
          Zainteresirani za najam vozila?
        </h3>

        <section class="pb-3 mb-3 mx-2 rounded-3 bg-white pt-3">
          <div class="col-md-12 mb-4">
            <div class="bg-light rounded-3 p-3">
              <div class="position-relative">
                Nudimo usluge prijevoza putnika u domaćem i međunarodnom prometu
                na svim relacijama od 0-24h, kombijem i osobnim vozilima s
                vozačem.
              </div>
            </div>
          </div>
          <section class="mx-3 bg-light px-4 py-3 rounded-5">
            <div class="row">
              <div class="col-md-6 my-2">
                <div class="bg-white rounded-4 p-3 hover-link">
                  <div class="position-relative">
                    <div class="pb-4 pb-md-0 pr-md-5 text-start">
                      <h4 class="mt-0 mb-2 fw-bold">Najam automobila</h4>
                      <span
                        class="fw-bold d-inline-block mt-0 mb-0 text-secondary"
                      >
                        Nudimo najam kvalitetnih automobila.
                      </span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-6 my-2">
                <div class="bg-white rounded-4 p-3 hover-link">
                  <div class="position-relative">
                    <div class="pb-4 pb-md-0 pr-md-5 text-start">
                      <h4 class="fw-bold mt-0 mb-2">Najam kombija (8+1)</h4>
                      <span
                        class="fw-bold d-inline-block mt-0 mb-0 text-secondary"
                      >
                        Nudimo najam kvalitetnih kombija (8+1).
                      </span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </section>
      </div>
    </section>
  </Transition>

  <footer class="text-center fixed-bottom bg-white">
    <p class="fw-bold p-0 m-0 rounded-3">&copy; 2023 Kvarner Tours d.o.o.</p>
  </footer>
</template>

<script setup>
import { onMounted, ref } from "vue";
const racTime = ref(false);

onMounted(() => {
  setTimeout(() => {
    racTime.value = true;
  }, 13000);
});
</script>

<style scoped>
html {
  height: 100vh;
}
.slide-fade-enter-active {
  transition: all 1.5s ease-in-out;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(100%);
  opacity: 0;
}

.dissapear-leave-active {
  transition: all 0.3s ease-in-out;
}

.dissapear-enter-from,
.dissapear-leave-to {
  transform: translateY(100%);
  opacity: 0;
}

.hover-link {
  box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 3px,
    rgba(0, 0, 0, 0.3) 0px 6px 12px -2px, rgba(0, 0, 0, 0.2) 0px -2px 0px inset;
}
.hover-link:hover {
  box-shadow: rgba(0, 0, 0, 0.4) 0px 1px 2px,
    rgba(0, 0, 0, 0.3) 0px 4px 6px -1px, rgba(0, 0, 0, 0.2) 0px -1px 0px inset;
}
.reveal-text {
  background: #32aac2;
  background: repeating-linear-gradient(
    to top right,
    #32aac2 28%,
    rgb(67, 94, 194) 84%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.button-shadow {
  text-shadow: 0.5px 0.5px black;
  box-shadow: rgba(0, 0, 0, 0.4) 0px 1px 2px,
    rgba(0, 0, 0, 0.3) 0px 4px 6px -1px, rgba(0, 0, 0, 0.2) 0px -1px 0px inset;
}

.card {
box-shadow: rgba(17, 17, 26, 0.1) 0px 1px 6px;
}
</style>
