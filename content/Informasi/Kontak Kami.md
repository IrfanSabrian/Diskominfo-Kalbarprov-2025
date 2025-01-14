---
author: Katheryn Fox
title: Kontak Kami
date: 2025-01-04T12:52:00
type: informasi
---

<section class="relative bg-white dark:bg-gray-800 p-8 rounded-xl border-2 border-gray-300 dark:border-gray-600 shadow-lg mx-auto max-w-4xl">
    <div class="absolute top-0 right-0 bottom-0 w-1/3 bg-customYellow rounded-r-xl hidden md:block"></div>
    <div class="p-2 w-full max-w-4xl flex flex-col md:flex-row relative z-10">
        <!-- Kotak Putih -->
        <div class="w-full md:w-2/3 p-4 mr-4">
            <form id="contactForm" onsubmit="return validateForm(event)">
                <div class="flex flex-col md:flex-row gap-4 mb-4">
                    <div class="w-full">
                        <label for="name" class="block text-lg font-bold text-gray-700 dark:text-gray-200">Nama Lengkap</label>
                        <input type="text" id="name" required class="mt-1 block w-full border border-gray-300 dark:border-gray-600 rounded-md shadow-sm p-2 focus:ring-green-500 focus:border-green-500 dark:bg-gray-700 dark:text-white">
                    </div>
                    <div class="w-full">
                        <label for="email" class="block text-lg font-bold text-gray-700 dark:text-gray-200">Alamat Email</label>
                        <input type="email" id="email" required class="mt-1 block w-full border border-gray-300 dark:border-gray-600 rounded-md shadow-sm p-2 focus:ring-green-500 focus:border-green-500 dark:bg-gray-700 dark:text-white">
                    </div>
                </div>
                <div class="mb-4">
                    <label class="block text-lg font-bold text-gray-700 dark:text-gray-200">Subjek</label>
                    <div class="grid grid-cols-2 gap-4 mt-2">
                        <div class="flex items-center">
                            <input type="radio" id="kerjasama" name="subjek" value="Kerjasama" required class="h-4 w-4 text-green-600 border-gray-300 dark:border-gray-600 focus:ring-green-500">
                            <label for="kerjasama" class="ml-2 block text-sm text-gray-700 dark:text-gray-200">Kerjasama</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" id="konten" name="subjek" value="Konten" class="h-4 w-4 text-green-600 border-gray-300 dark:border-gray-600 focus:ring-green-500">
                            <label for="konten" class="ml-2 block text-sm text-gray-700 dark:text-gray-200">Konten</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" id="pengaduan" name="subjek" value="Pengaduan" class="h-4 w-4 text-green-600 border-gray-300 dark:border-gray-600 focus:ring-green-500">
                            <label for="pengaduan" class="ml-2 block text-sm text-gray-700 dark:text-gray-200">Pengaduan</label>
                        </div>
                        <div class="flex items-center">
                            <input type="radio" id="lainnya" name="subjek" value="Lainnya" class="h-4 w-4 text-green-600 border-gray-300 dark:border-gray-600 focus:ring-green-500">
                            <label for="lainnya" class="ml-2 block text-sm text-gray-700 dark:text-gray-200">Lainnya</label>
                        </div>
                    </div>
                </div>
                <div class="mb-4">
                    <label for="message" class="block text-lg font-bold text-gray-700 dark:text-gray-200">Pesan</label>
                    <textarea id="message" rows="4" required class="mt-1 block w-full border border-gray-300 dark:border-gray-600 rounded-md shadow-sm p-2 focus:ring-green-500 focus:border-green-500 resize-none dark:bg-gray-700 dark:text-white"></textarea>
                </div>
                <button type="submit" class="w-full bg-customGreen text-white py-2 rounded-md hover:bg-green-700">Kirim</button>
            </form>
        </div>
        <!-- Kotak Hijau -->
        <div class="w-full md:w-1/2 bg-customGreen dark:bg-green-700 text-white p-4 mt-4 md:mt-0 md:ml-4 relative z-20">
            <h2 class="text-lg font-bold mb-2">Informasi Kami</h2>
            <p class="mb-4 font-medium text-sm">Isi form ini dan kami akan memberikan respon maksimal dalam 1 hari kerja.</p>
            <div class="flex items-center mb-2">
                <i class="fas fa-map-marker-alt mr-2 text-xl"></i>
                <span class="font-medium text-sm">Kantor Gubernur Kalimantan Barat</span>
            </div>
            <div class="flex items-center mb-2">
                <i class="fas fa-phone-alt mr-2 text-xl"></i>
                <span class="font-medium text-sm">+6289699305225</span>
            </div>
            <div class="flex items-center mb-4">
                <i class="fas fa-envelope mr-2 text-xl"></i>
                <span class="font-medium text-sm">diskominfo@kalbarprov.go.id</span>
            </div>
            <div class="flex flex-wrap gap-3 justify-center">
                <a href="https://www.youtube.com/@DiskominfoProvKalbar" target="_blank" class="text-customGreen dark:text-green-700 hover:text-green-800 dark:hover:text-green-900 w-10 h-10 rounded-full bg-white dark:bg-gray-200 flex items-center justify-center flex-shrink-0">
                    <i class="fab fa-youtube text-2xl"></i>
                </a>
                <a href="https://www.facebook.com/Diskominfoprovkalbar" target="_blank" class="text-customGreen dark:text-green-700 hover:text-green-800 dark:hover:text-green-900 w-10 h-10 rounded-full bg-white dark:bg-gray-200 flex items-center justify-center flex-shrink-0">
                    <i class="fab fa-facebook text-2xl"></i>
                </a>
                <a href="https://www.tiktok.com/@diskominfo.kalbar" target="_blank" class="text-customGreen dark:text-green-700 hover:text-green-800 dark:hover:text-green-900 w-10 h-10 rounded-full bg-white dark:bg-gray-200 flex items-center justify-center flex-shrink-0">
                    <i class="fab fa-tiktok text-2xl"></i>
                </a>
                <a href="https://x.com/KominfoKalbar" target="_blank" class="text-customGreen dark:text-green-700 hover:text-green-800 dark:hover:text-green-900 w-10 h-10 rounded-full bg-white dark:bg-gray-200 flex items-center justify-center flex-shrink-0">
                    <i class="fab fa-twitter text-2xl"></i>
                </a>
                <a href="https://www.instagram.com/diskominfo.kalbar/" target="_blank" class="text-customGreen dark:text-green-700 hover:text-green-800 dark:hover:text-green-900 w-10 h-10 rounded-full bg-white dark:bg-gray-200 flex items-center justify-center flex-shrink-0">
                    <i class="fab fa-instagram text-2xl"></i>
                </a>
            </div>
        </div>
    </div>
</section>

<script>
function validateForm(event) {
    event.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;
    const subjekRadios = document.getElementsByName('subjek');
    let selectedSubjek = '';
    
    for (let radio of subjekRadios) {
        if (radio.checked) {
            selectedSubjek = radio.value;
            break;
        }
    }
    
    if (!name || !email || !message || !selectedSubjek) {
        alert('Mohon lengkapi semua field yang diperlukan');
        return false;
    }
    
    const emailBody = `Nama: ${name}\nEmail: ${email}\nSubjek: ${selectedSubjek}\nPesan: ${message}`;
    
    const mailtoLink = `mailto:diskominfo@kalbarprov.go.id?subject=${encodeURIComponent(selectedSubjek)}&body=${encodeURIComponent(emailBody)}`;
    
    window.location.href = mailtoLink;
    return false;
}
</script>