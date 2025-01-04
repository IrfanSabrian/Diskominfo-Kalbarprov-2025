---
author: Katheryn Fox
title: Layanan
date: 2025-01-04T12:54:00
type: informasi
---

<script>
  function titleToUrl(title) {
    return title.toLowerCase().replace(/ /g, '-').replace(/[^\w-]+/g, '');
  }

  const layanan = [
    {
      title: "Sikedip",
      eurl: "https://sikedip.kalbarprov.go.id/",
      thumbnail: "/images/sikedip.jpeg", 
      logo: "/images/sikedip_logo.png"
    },
    {
      title: "PPID Utama",
      eurl: "https://ppid.kalbarprov.go.id/",
      thumbnail: "/images/ppid.jpeg",
      logo: "/images/ppid_logo.png"
    },
    {
      title: "Lapor",
      eurl: "https://www.lapor.go.id/",
      thumbnail: "/images/lapor.jpeg",
      logo: "/images/lapor_logo.png"
    }
  ];

  // Render layanan cards
  document.write('<div class="layanan-container">');
  layanan.forEach(item => {
    const card = `
      <div class="grid-item blog-card-layanan relative text-white rounded-lg shadow-md overflow-hidden p-4" 
           style="width: 280px; height: 160px;">
        <a href="${item.eurl}" class="absolute inset-0" target="_blank">
          <div class="thumbnail-container-layanan" 
               style="background-image: url('${item.thumbnail}'); padding: 20px; background-size: cover; background-repeat: no-repeat; background-position: center;"
               loading="lazy">
            <div class="dark-overlay-layanan"></div>
            <div class="logo-container-layanan">
              <img src="${item.logo}" class="logo-image-layanan" alt="${item.title} logo" loading="lazy">
            </div>
            <div class="eurl-overlay-layanan" style="padding: 10px;">
              <span class="eurl-text-layanan">${item.eurl}</span>
            </div>
            <div class="green-overlay-layanan"></div>
          </div>
        </a>
      </div>
    `;
    document.write(card);
  });
  document.write('</div>');
</script>

<style>
  .layanan-container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
    padding: 15px;
  }

  .blog-card-layanan {
    background-size: cover;
    background-position: center;
    display: inline-block;
  }

  .thumbnail-container-layanan {
    position: absolute;
    inset: 0;
    transition: background-color 0.3s ease, transform 0.3s ease, background-image 0.3s ease;
  }

  .logo-container-layanan {
    position: absolute;
    inset: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: opacity 0.3s ease;
  }

  .logo-image-layanan {
    max-width: 55%;
    max-height: 55%;
    object-fit: contain;
  }

  .dark-overlay-layanan {
    position: absolute;
    inset: 0;
    background-color: rgba(0, 0, 0, 0.4);
  }

  .eurl-overlay-layanan {
    position: absolute;
    inset: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .eurl-text-layanan {
    color: white;
    font-size: 0.95rem;
    font-weight: bold;
    padding: 6px;
    word-wrap: break-word;
    max-width: 100%;
  }

  .green-overlay-layanan {
    position: absolute;
    inset: 0;
    background-color: #03a055;
    opacity: 0;
    transition: opacity 0.3s ease;
    z-index: -1;
  }

  .thumbnail-container-layanan:hover .logo-container-layanan {
    opacity: 0;
  }

  .thumbnail-container-layanan:hover .dark-overlay-layanan {
    display: none;
  }

  .thumbnail-container-layanan:hover .eurl-overlay-layanan {
    opacity: 1;
  }

  .thumbnail-container-layanan:hover .green-overlay-layanan {
    opacity: 0.5;
  }

  .thumbnail-container-layanan:hover {
    transform: scale(1.10);
  }

  @media (max-width: 768px) {
    .blog-card-layanan {
      width: 100%;
      height: auto;
      aspect-ratio: 16 / 9;
    }
  }
</style>
