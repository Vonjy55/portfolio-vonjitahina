<template>
  <div class="container-xxl py-6" id="about">
    <div class="container">
        <div class="row g-5">
            <div class="col-lg-6 wow fadeInUp" data-wow-delay="0.1s">
                <div class="d-flex align-items-center mb-5">
                    <div class="years flex-shrink-0 text-center me-4">
                        <h1 class="display-1 mb-0">5</h1>
                        <h5 class="mb-0">{{ $t('about.years') }}</h5>
                    </div>
                    <h3 class="lh-base mb-0">{{ $t('about.exp_title') }}</h3>
                </div>
                <p class="mb-4">{{ $t('about.desc1') }}</p>
                <p class="mb-3"><i class="far fa-check-circle text-primary me-3"></i>{{ $t('about.point1') }}</p>
                <p class="mb-3"><i class="far fa-check-circle text-primary me-3"></i>{{ $t('about.point2') }}</p>
                <p class="mb-3"><i class="far fa-check-circle text-primary me-3"></i>{{ $t('about.point3') }}</p>
                <a class="btn btn-primary py-3 px-5 mt-3" href="#contact">{{ $t('about.btn_contact') }}</a>
            </div>
            <div class="col-lg-6 wow fadeInUp" data-wow-delay="0.5s">
                <div class="d-flex align-items-center mb-3">
                    <h5 class="fw-bold mb-0 text-dark" style="font-size: 1.1rem;">{{ $t('about.projects_completed') }}</h5>
                    <div class="ms-3 ps-3 border-start border-primary border-2">
                        <h3 class="text-primary mb-0" style="font-size: 1.75rem;">4</h3>
                    </div>
                </div>
                <p class="mb-4 text-dark" style="line-height: 1.6; font-size: 0.95rem;">{{ $t('about.desc2') }}</p>

                <div class="row g-3 mb-4">
                    <div class="col-md-4">
                        <div class="bg-light rounded p-3 h-100" style="background-color: #f8f9fa !important;">
                            <h3 class="text-primary mb-1 fw-bold" style="font-size: 1.5rem;">{{ $t('about.stat_years.val') }}</h3>
                            <span class="text-dark small lh-sm d-block">{{ $t('about.stat_years.desc') }}</span>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="bg-light rounded p-3 h-100" style="background-color: #f8f9fa !important;">
                            <h3 class="text-primary mb-1 fw-bold" style="font-size: 1.5rem;">{{ $t('about.stat_countries.val') }}</h3>
                            <span class="text-dark small lh-sm d-block">{{ $t('about.stat_countries.desc') }}</span>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="bg-light rounded p-3 h-100" style="background-color: #f8f9fa !important;">
                            <h3 class="text-primary mb-1 fw-bold" style="font-size: 1.5rem;">{{ $t('about.stat_tech.val') }}</h3>
                            <span class="text-dark small lh-sm d-block">{{ $t('about.stat_tech.desc') }}</span>
                        </div>
                    </div>
                </div>

                <hr class="w-100 mt-4 mb-4" style="border-color: #dee2e6;">
                
                <p class="text-uppercase fw-bold text-muted small mb-3" style="letter-spacing: 1px; font-size: 0.75rem;">{{ $t('about.companies') }}</p>

                <div class="row g-3">
                    <div class="col-md-4">
                        <div class="border rounded p-2 d-flex align-items-center bg-white h-100 w-100">
                            <div class="rounded d-flex align-items-center justify-content-center me-3 flex-shrink-0" style="width: 35px; height: 35px; background-color: rgba(102, 16, 242, 0.1); color: #6610f2; font-weight: 700;">
                                M
                            </div>
                            <div>
                                <h6 class="mb-0 fw-bold" style="font-size: 0.85rem; color: #343a40;">Mautourco</h6>
                                <small class="text-muted d-block" style="font-size: 0.75rem;">Maurice • 3 ans</small>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="border rounded p-2 d-flex align-items-center bg-white h-100 w-100">
                            <div class="rounded d-flex align-items-center justify-content-center me-3 flex-shrink-0" style="width: 35px; height: 35px; background-color: rgba(32, 201, 151, 0.1); color: #20c997; font-weight: 700;">
                                B
                            </div>
                            <div>
                                <h6 class="mb-0 fw-bold" style="font-size: 0.85rem; color: #343a40;">BICI</h6>
                                <small class="text-muted d-block" style="font-size: 0.75rem;">Madagascar • 1 an</small>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="border rounded p-2 d-flex align-items-center bg-white h-100 w-100">
                            <div class="rounded d-flex align-items-center justify-content-center me-3 flex-shrink-0" style="width: 35px; height: 35px; background-color: rgba(253, 126, 20, 0.1); color: #fd7e14; font-weight: 700;">
                                N
                            </div>
                            <div>
                                <h6 class="mb-0 fw-bold" style="font-size: 0.85rem; color: #343a40;">Numerika Center</h6>
                                <small class="text-muted d-block" style="font-size: 0.75rem;">Antananarivo • 1 an</small>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>
</script>
