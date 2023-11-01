<template>
    <!-- Header Section -->
    <header class="bg-light text-center pb-5">
      <div class="container">
        <img
          width="150px"
          src="../assets/imgs/kt.png"
          alt="Taxi Service"
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
    <!-- Service Highlights -->
<section class="py-3 mb-3 rounded-bottom-3 mx-2 bg-light">
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card mb-4 shadow border border-1 rounded-5 border-secondary">
          <div class="card-body">
            <h2 class="card-title">0-24h</h2>
            <p class="card-text">
              Pozovite vožnju bilo kada, bio dan ili noć.
            </p>
          </div>
        </div>
      </div>
      <!-- <div class="col-md-4">
        <div class="card mb-4 shadow">
          <div class="card-body">
            <h2 class="card-title">Iskusni Vozači</h2>
            <p class="card-text">
              Iskusni vozači osposobljeni za vašu sigurnost.
            </p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card mb-4 shadow">
          <div class="card-body">
            <h2 class="card-title">Visoki Standardi</h2>
            <p class="card-text">
              Svako vozilo je podvrgnuto detaljnom čišćenju i redovitom održavanju radi vaše sigurnosti i udobnosti.
            </p>
          </div>
        </div>
      </div> -->
    </div>
  </div>
</section>

    <section class="py-3 mx-2 mx-1 rounded-5 rounded-bottom-0 shadow-lg mb-5 bg-white">
      <div class="container">
                <img
          width="200px"
          src="../assets/imgs/kt.png"
          alt="Taxi Service"
          class="img-fluid mb-4"
        />
        <h3 class="fs-1 reveal-text fw-bold">
          Zainteresiran za najam vozila?
        </h3>
        <p class="lead mx-2">Ne kompliciraj.</p>
    <section class="pb-3 mb-3 mx-2 rounded-3 bg-white pt-3 mb-5 pb-5">
                          <div class="col-md-12 mb-4">
            <div class="bg-light rounded-3 p-3">
              <div class="position-relative">
                Nudimo usluge prijevoza putnika u domaćem i međunarodnom prometu na
                svim relacijama od 0-24h, kombijem i osobnim vozilima s vozačem.
              </div>
            </div>
          </div>
      <section class="mx-3 bg-light p-4 rounded-5">
        <div class="row">
          <div class="col-md-6 mb-4">
            <div class="bg-white shadow rounded-3 p-3">
              <div class="position-relative">
                <div class="pb-4 pb-md-0 pr-md-5 text-start">
                  <h5 class="mt-0 mb-2 fw-bold">Najam automobila</h5>
                  <span class="fw-bold d-inline-block mt-0 mb-0 text-secondary">
                    Nudimo najam kvalitetnih automobila.</span
                  >
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-6 mb-4">
            <div class="bg-white shadow rounded-3 p-3">
              <div class="position-relative">
                <div class="pb-4 pb-md-0 pr-md-5 text-start">
                  <h5 class="fw-bold mt-0 mb-2">Najam kombija (8+1)</h5>
                  <span class="fw-bold d-inline-block mt-0 mb-0 text-secondary"
                    >Nudimo najam kvalitetnih kombija (8+1).</span
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </section>

      </div>
    </section>


    <!-- Footer -->
    <footer class="text-center fixed-bottom bg-white">
      <p class="fw-bold p-0 m-0 rounded-3">&copy; 2023 Kvarner Tours d.o.o.</p>
    </footer>
</template>

<script setup></script>

<style>
html {
  height: 100vh;
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
  box-shadow: rgba(6, 24, 44, 0.4) 0px 0px 0px 2px,
    rgba(6, 24, 44, 0.65) 0px 4px 6px -1px,
    rgba(255, 255, 255, 0.08) 0px 1px 0px inset;
}
</style>
