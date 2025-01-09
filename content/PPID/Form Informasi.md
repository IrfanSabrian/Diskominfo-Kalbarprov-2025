---
author: Katheryn Fox
title: Form Informasi 
date: 2025-01-04T12:56:00
---

<script>
const formInformasiPPID = [
  {
    title: "Form Permintaan Informasi",
    icon: '/icon/form-permintaan-informasi.png',
    description: "Formulir yang dapat digunakan untuk memberikan permohonan terkait informasi yang belum tersedia.",
    buttonText: "Ajukan Permintaan",
    url: "https://layanan-diskominfo.kalbarprov.go.id/PPIDKALBAR-PERMOHONAN/register",
    target: "_blank"
  },
  {
    title: "Form Pernyataan Keberatan", 
    icon: '/icon/form-pernyataan-keberatan.png',
    description: "Formulir yang dapat digunakan untuk menyatakan keberatan terhadap permintaan informasi yang sudah ada.",
    buttonText: "Ajukan Pernyataan",
    url: "https://layanan-diskominfo.kalbarprov.go.id/PPIDKALBAR-KEBERATAN/register",
    target: "_blank"
  },
  {
    title: "Daftar Form",
    icon: '/icon/daftar-form.png',
    description: "Kumpulan formulir yang tersedia untuk berbagai keperluan layanan informasi publik yang dapat diunduh.",
    buttonText: "Daftar Formulir",
    url: "/ms-form-informasi-ppid/daftar-form",
    target: "_self"
  }
];

document.addEventListener("DOMContentLoaded", function() {
  const containerFormInformasiPPID = document.querySelector('.section-container-form-informasi-ppid');
  formInformasiPPID.forEach(item => {
    containerFormInformasiPPID.innerHTML += `
      <div class="form-card bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6 text-center flex flex-col justify-between border-2 border-gray-200 dark:border-gray-600" style="width: 260px; height: auto; min-height: 358px;">
        <div>
          <div class="flex justify-center mb-4">
            <img src="${item.icon}" alt="${item.title}" class="w-16 h-16"/>
          </div>
          <h2 class="text-xl font-semibold mb-2 text-black dark:text-white">${item.title}</h2>
          <p class="text-gray-600 dark:text-gray-300 mb-6">${item.description}</p>
        </div>
        <a href="${item.url}" target="${item.target}" class="bg-customGreen text-white font-semibold py-2 px-4 rounded-full hover:bg-green-700">
          ${item.buttonText}
        </a>
      </div>
    `;
  });
});
</script>

<section class="flex flex-row flex-wrap md:flex-nowrap gap-6 justify-center items-stretch p-6 section-container-form-informasi-ppid">
</section>

<style>
@media (max-width: 768px) {
  .section-container-form-informasi-ppid {
    flex-direction: column;
    align-items: center;
  }
  .form-card {
    width: 100% !important;
  }
}
</style>