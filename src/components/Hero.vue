<template>
  <div class="container-fluid bg-light my-6 mt-0" id="home">
    <div class="container">
        <div class="row g-5 align-items-center">
            <div class="col-lg-6 py-6 pb-0 pt-lg-0">
                <h3 class="text-primary mb-3">{{ $t('hero.im') }}</h3>
                <h1 class="display-3 mb-3">Ranjelison Vonjitahina Charles</h1>
                <h2 class="typed-text-output d-inline"></h2>
                <div class="typed-text d-none">{{ $t('hero.roles') }}</div>
                <div class="d-flex align-items-center pt-5">
                    <a href="/cv/CV-Ranjelison-Vonjitahina-BE.pdf" target="_blank" download="CV-Ranjelison-Vonjitahina.pdf" class="btn btn-primary py-3 px-4 me-5">{{ $t('hero.download_cv') }}</a>
                </div>
            </div>
            <div class="col-lg-6">
                <!-- Keep placeholder for now or replace with an avatar later -->
                <img class="img-fluid" src="/img/profile.png" alt="Profile">
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>
</script>
