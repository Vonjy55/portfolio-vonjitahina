<template>
  <div class="container-xxl py-6" id="services">
    <div class="container">
      <!-- Section Header -->
      <div class="text-center wow fadeInUp mb-5" data-wow-delay="0.1s">
        <h1 class="display-5 mb-3">{{ $t('services.title') }}</h1>
        <p class="text-muted">{{ $t('services.subtitle') }}</p>
      </div>

      <!-- Cards -->
      <div class="row g-4 justify-content-center wow fadeInUp" data-wow-delay="0.2s">
        <!-- Card 1 — Web Development -->
        <div class="col-lg col-md-6 col-sm-12">
          <div class="service-card h-100">
            <div class="service-icon s-icon-1 mb-4">
              <i class="fa fa-code"></i>
            </div>
            <h5 class="fw-bold mb-3">{{ $t('services.s1_title') }}</h5>
            <p class="text-muted mb-0">{{ $t('services.s1_desc') }}</p>
          </div>
        </div>
        <!-- Card 2 — REST API -->
        <div class="col-lg col-md-6 col-sm-12">
          <div class="service-card h-100">
            <div class="service-icon s-icon-2 mb-4">
              <i class="fa fa-server"></i>
            </div>
            <h5 class="fw-bold mb-3">{{ $t('services.s2_title') }}</h5>
            <p class="text-muted mb-0">{{ $t('services.s2_desc') }}</p>
          </div>
        </div>
        <!-- Card 3 — AI & ML -->
        <div class="col-lg col-md-6 col-sm-12">
          <div class="service-card h-100">
            <div class="service-icon s-icon-3 mb-4">
              <i class="fa fa-brain"></i>
            </div>
            <h5 class="fw-bold mb-3">{{ $t('services.s3_title') }}</h5>
            <p class="text-muted mb-0">{{ $t('services.s3_desc') }}</p>
          </div>
        </div>
        <!-- Card 4 — IA Automation -->
        <div class="col-lg col-md-6 col-sm-12">
          <div class="service-card h-100">
            <div class="service-icon s-icon-4 mb-4">
              <i class="fa fa-robot"></i>
            </div>
            <h5 class="fw-bold mb-3">{{ $t('services.s4_title') }}</h5>
            <p class="text-muted mb-0">{{ $t('services.s4_desc') }}</p>
          </div>
        </div>
        <!-- Card 5 — Data Visualization -->
        <div class="col-lg col-md-6 col-sm-12">
          <div class="service-card h-100">
            <div class="service-icon s-icon-5 mb-4">
              <i class="fa fa-chart-bar"></i>
            </div>
            <h5 class="fw-bold mb-3">{{ $t('services.s5_title') }}</h5>
            <p class="text-muted mb-0">{{ $t('services.s5_desc') }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.service-card {
  background: #fff;
  border: 1px solid #ede8f9;
  border-top: 3px solid var(--primary);
  border-radius: 8px;
  padding: 1.5rem;
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.service-card:hover {
  box-shadow: 0 8px 32px rgba(98, 68, 197, 0.13);
  transform: translateY(-5px);
}

.service-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 52px;
  height: 52px;
  border-radius: 12px;
  font-size: 1.3rem;
}

.s-icon-1 {
  background: rgba(98, 68, 197, 0.10);
  color: var(--primary);
}

.s-icon-2 {
  background: rgba(255, 196, 72, 0.15);
  color: #c48a00;
}

.s-icon-3 {
  background: rgba(98, 68, 197, 0.10);
  color: var(--primary);
}

.s-icon-4 {
  background: rgba(255, 196, 72, 0.15);
  color: #c48a00;
}

.s-icon-5 {
  background: rgba(32, 201, 151, 0.12);
  color: #159a6e;
}
</style>
