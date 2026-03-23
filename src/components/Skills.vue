<template>
  <div class="container-xxl py-6 pb-5" id="skill">
    <div class="container">
        <div class="row g-5">
            <div class="col-lg-6 wow fadeInUp" data-wow-delay="0.1s">
                <h1 class="display-5 mb-5">{{ $t('skills.title') }}</h1>
                <p class="mb-4">{{ $t('skills.subtitle') }}</p>
                <h3 class="mb-4">{{ $t('skills.my_skills') }}</h3>
                <!-- LANGAGES & FRAMEWORKS -->
                <h6 class="text-uppercase text-muted fw-bold mb-4 mt-2" style="letter-spacing: 1px; font-size: 0.8rem;">{{ $t('skills.cat_lang_fw') }}</h6>
                <div class="row g-4 mb-5">
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">Python</h6>
                                <span class="fw-bold text-muted small">95%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 95%; background-color: #7B61FF;" aria-valuenow="95" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Django</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">FastAPI</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Flask</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">JavaScript</h6>
                                <span class="fw-bold text-muted small">85%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 85%; background-color: #F59E0B;" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Angular</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Vue.js</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">ES6+</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">PHP</h6>
                                <span class="fw-bold text-muted small">85%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 85%; background-color: #E25822;" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Laravel</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">Machine Learning / IA</h6>
                                <span class="fw-bold text-muted small">80%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 80%; background-color: #20C997;" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Scikit-learn</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Pandas</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Numpy</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Tensorflow</span>
                            </div>
                        </div>
                    </div>
                </div>

                <hr class="w-100 mb-4" style="border-color: #dee2e6;">

                <!-- DONNÉES & INFRASTRUCTURE -->
                <h6 class="text-uppercase text-muted fw-bold mb-4" style="letter-spacing: 1px; font-size: 0.8rem;">{{ $t('skills.cat_data_infra') }}</h6>
                <div class="row g-4 mb-4">
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">{{ $t('skills.db_title') }}</h6>
                                <span class="fw-bold text-muted small">90%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 90%; background-color: #3B82F6;" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">PostgreSQL</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">MySQL</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">NoSQL</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">Data & Visualisation</h6>
                                <span class="fw-bold text-muted small">75%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 75%; background-color: #8A817C;" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Power BI</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Pandas</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Numpy</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">Docker / Git / CI-CD</h6>
                                <span class="fw-bold text-muted small">90%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 90%; background-color: #8A817C;" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">GitHub Actions</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Git</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">AWS Cloud</h6>
                                <span class="fw-bold text-muted small">80%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 80%; background-color: #F59E0B;" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">EC2</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">RDS</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">S3</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">API REST</h6>
                                <span class="fw-bold text-muted small">95%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 95%; background-color: #7B61FF;" aria-valuenow="95" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Design</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">{{ $t('skills.integration') }}</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Documentation</span>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="skill">
                            <div class="d-flex justify-content-between mb-2">
                                <h6 class="fw-bold mb-0">{{ $t('skills.automatisation') }}</h6>
                                <span class="fw-bold text-muted small">75%</span>
                            </div>
                            <div class="progress mb-2" style="height: 6px; border-radius: 10px;">
                                <div class="progress-bar" role="progressbar" style="width: 75%; background-color: #7B61FF;" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="d-flex flex-wrap gap-2">
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">n8n</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Scripts Python</span>
                                <span class="badge text-muted fw-normal rounded-pill" style="background-color: #f4f5f7; font-size: 0.75rem; padding: 0.35rem 0.7rem;">Workflows</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-lg-6 wow fadeInUp" data-wow-delay="0.5s">
                <ul class="nav nav-pills rounded border border-2 border-primary mb-5">
                    <li class="nav-item w-50">
                        <button class="nav-link w-100 py-3 fs-5 active" data-bs-toggle="pill" data-bs-target="#tab-1">{{ $t('skills.tab_exp') }}</button>
                    </li>
                    <li class="nav-item w-50">
                        <button class="nav-link w-100 py-3 fs-5" data-bs-toggle="pill" data-bs-target="#tab-2">{{ $t('skills.tab_edu') }}</button>
                    </li>
                </ul>
                <div class="tab-content">
                    <div id="tab-1" class="tab-pane fade show p-0 active">
                        <div class="row gy-5 gx-4">
                            <div class="col-sm-12">
                                <h5>{{ $t('skills.exp1_title') }}</h5>
                                <hr class="text-primary my-2">
                                <p class="text-primary mb-1">{{ $t('skills.exp1_dur') }}</p>
                                <h6 class="mb-0">{{ $t('skills.exp1_loc') }}</h6>
                                <small>{{ $t('skills.exp1_desc') }}</small>
                            </div>
                            <div class="col-sm-12">
                                <h5>{{ $t('skills.exp2_title') }}</h5>
                                <hr class="text-primary my-2">
                                <p class="text-primary mb-1">{{ $t('skills.exp2_dur') }}</p>
                                <h6 class="mb-0">{{ $t('skills.exp2_loc') }}</h6>
                                <small>{{ $t('skills.exp2_desc') }}</small>
                            </div>
                            <div class="col-sm-12">
                                <h5>{{ $t('skills.exp3_title') }}</h5>
                                <hr class="text-primary my-2">
                                <p class="text-primary mb-1">{{ $t('skills.exp3_dur') }}</p>
                                <h6 class="mb-0">{{ $t('skills.exp3_loc') }}</h6>
                                <small>{{ $t('skills.exp3_desc') }}</small>
                            </div>
                        </div>
                    </div>
                    <div id="tab-2" class="tab-pane fade show p-0">
                        <div class="row gy-5 gx-4">
                            <div class="col-sm-12">
                                <h5>{{ $t('skills.edu1_title') }}</h5>
                                <hr class="text-primary my-2">
                                <p class="text-primary mb-1">{{ $t('skills.edu1_year') }}</p>
                                <h6 class="mb-0">{{ $t('skills.edu1_loc') }}</h6>
                                <small>{{ $t('skills.edu1_desc') }}</small>
                            </div>
                            <div class="col-sm-12">
                                <h5>{{ $t('skills.edu2_title') }}</h5>
                                <hr class="text-primary my-2">
                                <p class="text-primary mb-1">{{ $t('skills.edu2_year') }}</p>
                                <h6 class="mb-0">{{ $t('skills.edu2_loc') }}</h6>
                                <small>{{ $t('skills.edu2_desc') }}</small>
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
