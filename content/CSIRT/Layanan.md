---
author: Katheryn Fox
title: Layanan
date: 2025-01-03T12:56:00
---

<script>
const formInformasiPPID = [
  {
    title: "Penanganan Kerawanan",
    icon: '/icon/penanganan-kerawanan-csirt.png',
    buttonText: "Selengkapnya",
    url: "/ms-layanan-csirt/penanganan-kerawanan",
    target: "_self"
  },
  {
    title: "Penanganan Insiden Siber",
    icon: '/icon/penanganan-insiden-siber-csirt.png',
    buttonText: "Selengkapnya",
    url: "/ms-layanan-csirt/penanganan-insiden-siber", 
    target: "_self"
  },
  {
    title: "Pemberian Peringatan Terkait Keamanan Siber",
    icon: '/icon/pemberian-peringatan-csirt.png',
    buttonText: "Selengkapnya",
    url: "/ms-layanan-csirt/pemberian-peringatan-terkait-keamanan-siber",
    target: "_self"
  }
];

document.addEventListener("DOMContentLoaded", function() {
  const containerFormInformasiPPID = document.querySelector('.section-container-form-informasi-ppid');
  formInformasiPPID.forEach(item => {
    containerFormInformasiPPID.innerHTML += `
      <div class="form-card bg-white rounded-lg shadow-lg p-6 text-center flex flex-col justify-between border-2 border-gray-200" style="width: 260px; height: auto; min-height: 358px;">
        <div>
          <div class="flex justify-center mb-4">
            <img src="${item.icon}" alt="${item.title}" class="w-32 h-32"/>
          </div>
          <h2 class="text-xl font-semibold mb-2">${item.title}</h2>
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