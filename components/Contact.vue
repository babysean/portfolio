<template>
  <section id="contact" class="py-20 bg-gray-100">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <h2 class="text-3xl font-bold text-gray-900">Get In Touch</h2>
        <div class="w-16 h-1 bg-indigo-600 mx-auto mt-4 mb-6"></div>
        <p class="text-gray-600 max-w-2xl mx-auto">Have a project in mind or want to collaborate? Feel free to contact me!</p>
      </div>
      <div class="flex flex-col md:flex-row gap-10">
        <div class="w-full">
          <div class="bg-white p-8 rounded-lg shadow-md h-full">
            <h3 class="text-2xl font-bold text-gray-900 mb-6">Contact Information</h3>
            <div class="space-y-6">
              <div class="flex items-start">
                <MapPinIcon class="h-6 w-6 text-indigo-600 mt-1 mr-4" />
                <div>
                  <h4 class="font-bold text-gray-900">Location</h4>
                  <p class="text-gray-600">Seoul, South Korea</p>
                </div>
              </div>
              <div class="flex items-start">
                <MailIcon class="h-6 w-6 text-indigo-600 mt-1 mr-4" />
                <div>
                  <h4 class="font-bold text-gray-900">Email</h4>
                  <p class="text-gray-600">your.email@example.com</p>
                </div>
              </div>
              <div class="flex items-start">
                <PhoneIcon class="h-6 w-6 text-indigo-600 mt-1 mr-4" />
                <div>
                  <h4 class="font-bold text-gray-900">Phone</h4>
                  <p class="text-gray-600">+82 10 0000 0000</p>
                </div>
              </div>
              <div class="pt-6">
                <h4 class="font-bold text-gray-900 mb-4">Follow Me</h4>
                <div class="flex space-x-4">
                  <a href="#" class="bg-indigo-100 p-3 rounded-full text-indigo-600 hover:bg-indigo-200 transition-colors">
                    <GithubIcon class="h-5 w-5" />
                  </a>
                  <a href="#" class="bg-indigo-100 p-3 rounded-full text-indigo-600 hover:bg-indigo-200 transition-colors">
                    <LinkedinIcon class="h-5 w-5" />
                  </a>
                  <a href="#" class="bg-indigo-100 p-3 rounded-full text-indigo-600 hover:bg-indigo-200 transition-colors">
                    <TwitterIcon class="h-5 w-5" />
                  </a>
                  <a href="#" class="bg-indigo-100 p-3 rounded-full text-indigo-600 hover:bg-indigo-200 transition-colors">
                    <InstagramIcon class="h-5 w-5" />
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';
import { MapPinIcon, MailIcon, PhoneIcon, GithubIcon, LinkedinIcon, TwitterIcon, InstagramIcon } from 'lucide-vue-next';

const contactForm = ref({
  name: '',
  email: '',
  subject: '',
  message: ''
});
  
const formSubmitting = ref(false);

const submitForm = () => {
  formSubmitting.value = true;
  setTimeout(() => {
    contactForm.value = { name: '', email: '', subject: '', message: '' };
    formSubmitting.value = false;
    
    alert('Thank you for your message! I will get back to you soon.');
  }, 1500);
};
</script>
