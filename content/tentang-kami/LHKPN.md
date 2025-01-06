---
author: Katheryn Fox
title: LHKPN
date: 2024-12-30T12:53:00
type: tentang-kami
---

<script>
  function titleToUrl(title) {
    return title.toLowerCase().replace(/ /g, '-').replace(/[^\w-]+/g, '');
  }

  const lhkpn = [
    {
      title: "LHKPN Kepala Dinas dan Sekretaris",
      imageSrc: "/images/lhkpn.png"
    },
    {
      title: "LHKPN Pejabat Eselon 3", 
      imageSrc: "/images/lhkpn.png"
    },
    {
      title: "LHKPN Pejabat Eselon 4",
      imageSrc: "/images/lhkpn.png"
    },
    {
      title: "Informasi Jumlah dan Persentase Wajib LHKPN",
      imageSrc: "/images/informasi_lhkpn.png"
    }
  ];

  document.addEventListener("DOMContentLoaded", function() {
    const container = document.querySelector('.section-container');
    lhkpn.forEach(item => {
      const urlPath = `/ms-lhkpn/${titleToUrl(item.title)}`;
      container.innerHTML += `
        <a href="${urlPath}" class="bg-white p-4 rounded-xl border border-gray-300 shadow-lg hover-container cursor-pointer" style="width: 100%;">
          <div class="flex items-center justify-between">
            <div class="flex items-center flex-1">
              <div class="relative rounded-lg" style="height: 120px; width: 180px; background-image: url('${item.imageSrc}'); background-repeat: no-repeat; background-position: center; background-size: cover;">
                <div style="background: rgba(0,0,0,0.5); width: 100%; height: 100%;" class="rounded-md absolute top-0 left-0"></div>
              </div>
              <div class="flex items-center flex-1">
                <h2 class="text-black md:text-xl text-base ml-6 pr-4 flex items-center" style="height: 100px">${item.title}</h2>
                <div class="border-r-2 border-gray-300 h-28 ml-auto hidden md:block"></div>
              </div>
            </div>
            <div class="hidden md:flex items-center justify-center h-full w-40">
              <div class="hover-arrow flex items-center justify-center text-black group">
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
<section class="flex flex-col gap-4 bg-white section-container">
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
