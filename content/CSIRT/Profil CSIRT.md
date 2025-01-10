---
author: Katheryn Fox
title: Profil CSIRT
date: 2025-01-06T12:55:00
type: csirt
---
<script>
const profilCSIRT = [
    {
        icon: '/icon/tentang-csirt.png',
        title: 'Tentang CSIRT',
        type: 'link',
        link: '/ms-profil-csirt/tentang'
    },
    {
        icon: '/icon/struktur-organisasi-csirt.png', 
        title: 'Struktur Organisasi',
        type: 'link',
        link: '/ms-profil-csirt/struktur-organisasi'
    },
    {
        icon: '/icon/visi-dan-misi-csirt.png',
        title: 'Visi dan Misi',
        type: 'link',
        link: '/ms-profil-csirt/visi-dan-misi'
    }
];

function renderSections() {
    const container = document.querySelector('.container-menu');
    profilCSIRT.forEach(section => {
        const div = document.createElement('div');
        div.className = 'flex flex-col items-center menu-container';
        
        const content = section.type === 'modal' 
            ? `<div onclick="openImgModal('${section.link}')" class="bg-customGreen rounded-xl p-2 menu-item transition-all duration-300 cursor-pointer" 
                style="z-index: 5; width: 100px; height: 100px; overflow: hidden; opacity: 0.8; display: flex; justify-content: center; align-items: center;">
                <img src="${section.icon}" alt="${section.title}" class="h-4/5 max-h-full w-auto object-contain">
               </div>`
            : `<a href="${section.link}" class="bg-customGreen rounded-xl p-2 menu-item transition-all duration-300 cursor-pointer" 
                style="z-index: 5; width: 100px; height: 100px; overflow: hidden; opacity: 0.8; display: flex; justify-content: center; align-items: center;">
                <img src="${section.icon}" alt="${section.title}" class="h-4/5 max-h-full w-auto object-contain">
               </a>`;
               
        div.innerHTML = `
            ${content}
            <p class="text-base text-black dark:text-white text-center w-full mt-2">${section.title}</p>
        `;
        
        container.appendChild(div);
    });
}

document.addEventListener('DOMContentLoaded', renderSections);
</script>

<style>
.menu-container:hover .menu-item {
    transform: scale(1.1);
    opacity: 1;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.menu-container:hover .menu-title {
    font-weight: bold;
    color: #2F855A;
}

.container-menu {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: center;
    gap: 2rem;
}

@media (max-width: 767px) {
    .container-menu {
        grid-template-columns: repeat(2, 1fr);
        gap: 1rem;
    }
    
    .container-menu > div {
        transform: none !important;
    }
}
</style>

<div class="container container-menu px-4 md:px-32 gap-2 mx-auto max-w-4xl">
</div>