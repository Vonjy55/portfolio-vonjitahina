<template>
  <div class="container-xxl pb-5" id="contact">
    <div class="container py-5">
        <div class="row g-5 mb-5 wow fadeInUp" data-wow-delay="0.1s">
            <div class="col-lg-6">
                <h1 class="display-5 mb-0">{{ $t('contact.title') }}</h1>
            </div>
            <!-- <div class="col-lg-6 text-lg-end">
                <a class="btn btn-primary py-3 px-5" href="mailto:vonjitahinaranjelison@gmail.com">{{ $t('contact.say_hello') }}</a>
            </div> -->
        </div>
        <div class="row g-5">
            <div class="col-lg-5 col-md-6 wow fadeInUp" data-wow-delay="0.1s">
                <p class="mb-2">{{ $t('contact.loc') }}</p>
                <h3 class="fw-bold">Anosy, Antananarivo</h3>
                <hr class="w-100">
                <p class="mb-2">{{ $t('contact.phone') }}</p>
                <h3 class="fw-bold">+261 34 11 517 76</h3>
                <hr class="w-100">
                <p class="mb-2">Email:</p>
                <h3 class="fw-bold fs-5">vonjitahinaranjelison@gmail.com</h3>
                <hr class="w-100">
                <p class="mb-2">{{ $t('contact.follow') }}</p>
                <div class="d-flex pt-2">
                    <a class="btn btn-square btn-primary me-2" target="_blank" href="https://www.linkedin.com/in/vonjitahina-ranjelison/"><i class="fab fa-linkedin-in"></i></a>
                    <a class="btn btn-square btn-primary me-2" href="#"><i class="fab fa-github"></i></a>
                </div>
            </div>
            <div class="col-lg-7 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
                <form @submit.prevent="sendEmail">
                    <div class="row g-3">
                        <div class="col-md-6">
                            <div class="form-floating">
                                <input type="text" class="form-control" id="name" v-model="formData.name" :placeholder="$t('contact.name')" required>
                                <label for="name">{{ $t('contact.name') }}</label>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="form-floating">
                                <input type="email" class="form-control" id="email" v-model="formData.email" :placeholder="$t('contact.email')" required>
                                <label for="email">{{ $t('contact.email') }}</label>
                            </div>
                        </div>
                        <div class="col-12">
                            <div class="form-floating">
                                <input type="text" class="form-control" id="subject" v-model="formData.subject" :placeholder="$t('contact.subject')" required>
                                <label for="subject">{{ $t('contact.subject') }}</label>
                            </div>
                        </div>
                        <div class="col-12">
                            <div class="form-floating">
                                <textarea class="form-control" :placeholder="$t('contact.message')" id="message" v-model="formData.message" style="height: 100px" required></textarea>
                                <label for="message">{{ $t('contact.message') }}</label>
                            </div>
                        </div>
                        <div class="col-12 mt-2">
                            <button class="btn btn-primary py-3 px-5" type="submit" :disabled="formStatus === 'sending'">
                                <span v-if="formStatus === 'sending'" class="spinner-border spinner-border-sm me-2" role="status" aria-hidden="true"></span>
                                {{ $t('contact.send') }}
                            </button>
                        </div>
                        <div class="col-12 mt-3" v-if="formStatus === 'success'">
                            <div class="alert alert-success m-0 p-3">
                                ✓ Message envoyé avec succès. Merci !
                            </div>
                        </div>
                        <div class="col-12 mt-3" v-if="formStatus === 'error'">
                            <div class="alert alert-danger m-0 p-3">
                                ⚠ Une erreur est survenue lors de l'envoi. Veuillez réessayer plus tard.
                            </div>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>
import { reactive, ref } from 'vue';
import emailjs from '@emailjs/browser';

const formData = reactive({
    name: '',
    email: '',
    subject: '',
    message: ''
});

const formStatus = ref(null);

const sendEmail = async () => {
    formStatus.value = 'sending';
    
    try {
        const templateParams = {
            from_name: formData.name,
            from_email: formData.email,
            subject: formData.subject,
            message: formData.message,
            to_name: 'Vonjitahina'
        };

        // TODO: Remplacez ces valeurs par vos vrais identifiants EmailJS
        const SERVICE_ID = 'service_elq7mdn';
        const TEMPLATE_ID = 'template_0izr376';
        const PUBLIC_KEY = '0fYQ1bTtoKYnd1t5d';

        await emailjs.send(SERVICE_ID, TEMPLATE_ID, templateParams, PUBLIC_KEY);
        
        formStatus.value = 'success';
        
        formData.name = '';
        formData.email = '';
        formData.subject = '';
        formData.message = '';
        
        // Hide success message after 6 seconds
        setTimeout(() => {
            if (formStatus.value === 'success') formStatus.value = null;
        }, 6000);
        
    } catch (error) {
        console.error('EmailJS Error:', error);
        formStatus.value = 'error';
    }
};
</script>
