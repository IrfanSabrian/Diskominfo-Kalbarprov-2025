---
author: Katheryn Fox
title: Lapor Insiden
date: 2025-01-01T12:56:00
type: csirt
---

<script>
  function titleToUrl(title) {
    return title.toLowerCase().replace(/ /g, '-').replace(/[^\w-]+/g, '');
  }

  const laporInsiden = [
    {
      title: "Lapor Insiden"
    }
  ];

  document.addEventListener("DOMContentLoaded", function() {
    const containerSopPeraturan = document.querySelector('.section-container-lapor-insiden');
    laporInsiden.forEach(item => {
      containerSopPeraturan.innerHTML += `
        <a href="https://insidensiber.kalbarprov.go.id/" target="_blank" class="bg-white dark:bg-gray-800 p-4 rounded-xl border border-gray-300 dark:border-gray-600 shadow-lg hover-container cursor-pointer" style="width: 100%;">
          <div class="flex items-center justify-between">
            <div class="flex items-center flex-1">
              <div class="flex items-center flex-1">
                <h2 class="text-black dark:text-white md:text-xl text-base pr-4 flex items-center" style="height: 100px">${item.title}</h2>
                <div class="border-r-2 border-gray-300 dark:border-gray-600 h-28 ml-auto hidden md:block"></div>
              </div>
            </div>
            <div class="hidden md:flex items-center justify-center h-full w-40">
              <div class="hover-arrow flex items-center justify-center text-black dark:text-white group">
                <span class="mr-3">Selengkapnya</span>
                <i class="fas fa-arrow-right"></i>
              </div>
            </div>
          </div>
        </a>
      `;
    });
  });
</script>
<section class="flex flex-col gap-4 bg-white dark:bg-gray-800 section-container-lapor-insiden">
</section>
<style>
.hover-container:hover .hover-arrow {
    color: #00A86B;
    transform: translateX(10px);
}
.hover-container:hover .hover-arrow i {
    animation: arrowMove 0.8s infinite;
}
.hover-arrow {
    display: inline-flex;
    align-items: center;
    transition: all 0.3s ease;
}
@keyframes arrowMove {
    0% {
        transform: translateX(0);
    }
    50% {
        transform: translateX(5px);
    }
    100% {
        transform: translateX(0);
    }
}
@media (max-width: 768px) {
    .hover-container {
        flex-direction: column;
    }
    .hover-arrow {
        display: none;
    }
}
</style>