---
author: Katheryn Fox
title: Struktur Diskominfo
date: 2024-12-30T12:55:00
---
<script>
const strukturDiskominfo = [
    {
        icon: '/icon/struktur-organisasi.png',
        title: 'Struktur Organisasi',
        type: 'modal',
        link: '/images/struktur-organisasi.png'
    },
    {
        icon: '/icon/tugas-dan-fungsi.png', 
        title: 'Tugas dan Fungsi',
        type: 'link',
        link: '/ms-struktur-diskominfo/tugas-dan-fungsi'
    },
    {
        icon: '/icon/visi-dan-misi.png',
        title: 'Visi dan Misi',
        type: 'link', 
        link: '/ms-struktur-diskominfo/visi-dan-misi'
    },
    {
        icon: '/icon/kedudukan-dan-alamat.png',
        title: 'Kedudukan dan Alamat',
        type: 'link',
        link: '/ms-struktur-diskominfo/kedudukan-dan-alamat'
    },
    {
        icon: '/icon/ruang-lingkup.png',
        title: 'Ruang Lingkup',
        type: 'modal',
        link: '/images/ruang-lingkup.png'
    },
    {
        icon: '/icon/unit-kerja.png',
        title: 'Unit Kerja',
        type: 'link',
        link: '/ms-struktur-diskominfo/unit-kerja'
    }
];

function renderSections() {
    const container = document.querySelector('.container-menu');
    strukturDiskominfo.forEach(section => {
        const div = document.createElement('div');
        div.className = 'flex flex-col items-center menu-container';
        
        const content = section.type === 'modal' 
            ? `<div onclick="openImgModal('${section.link}')" class="bg-customGreen dark:bg-green-600 rounded-xl p-2 menu-item transition-all duration-300 cursor-pointer" 
                style="z-index: 5; width: 100px; height: 100px; overflow: hidden; opacity: 0.8; display: flex; justify-content: center; align-items: center;">
                <img src="${section.icon}" alt="${section.title}" class="h-4/5 max-h-full w-auto object-contain">
               </div>`
            : `<a href="${section.link}" class="bg-customGreen dark:bg-green-600 rounded-xl p-2 menu-item transition-all duration-300 cursor-pointer" 
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

@media (prefers-color-scheme: dark) {
    .menu-container:hover .menu-title {
        color: #48BB78;
    }
}
</style>

<div class="container container-menu px-4 gap-1 mx-0 grid grid-cols-2 md:grid-cols-3 bg-white dark:bg-gray-800">
</div>