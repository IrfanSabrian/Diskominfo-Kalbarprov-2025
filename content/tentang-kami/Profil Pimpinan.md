---
author: Katheryn Fox
title: Profil Pimpinan
date: 2024-12-30T12:56:00
---
<div class="max-w-4xl mx-auto bg-white dark:bg-gray-800 rounded-lg overflow-hidden">
    <div class="flex flex-col sm:flex-row">
        <div class="sm:w-1/3 w-full p-4 flex flex-col items-center">
            <img alt="Profil Pimpinan" class="w-3/4 sm:w-full rounded-lg mb-4" height="150" src="/images/pimpinanfix.png" width="150"/>
            <!-- Nama dan jabatan untuk tampilan mobile -->
            <div class="sm:hidden mb-4 text-center">
                <div class="text-2xl font-bold text-green-600 dark:text-green-400">SAMUEL, SE, M.Si</div>
                <div class="text-sm text-gray-600 dark:text-gray-300">Kepala Dinas Komunikasi dan Informatika Provinsi Kalimantan Barat</div>
            </div>
            <div class="flex items-center mb-2 w-full">
                <div class="text-left text-lg font-semibold text-green-600 dark:text-green-400">
                    Riwayat Pekerjaan
                </div>
                <div class="border-t-4 border-green-600 dark:border-green-400 flex-grow ml-2"></div>
            </div>
            <div class="bg-white dark:bg-gray-800 p-4 rounded-lg shadow border-2 border-gray-300 dark:border-gray-600 space-y-4 overflow-y-scroll w-full" style="height: 300px;">
                <div class="border-b border-gray-200 dark:border-gray-600 pb-4 mb-4">
                    <div class="flex justify-between items-center mb-2">
                        <div class="text-base font-semibold dark:text-white">Kepala Urusan Keuangan</div>
                        <div class="text-sm text-white bg-customGreen dark:bg-green-600 rounded-full px-4 py-1 inline-block text-center font-bold">1998</div>
                    </div>
                    <div class="mt-2 text-sm text-gray-500 dark:text-gray-400">Kepala Urusan Keuangan Pada Dinas Pasar Kab Daerah Tk. II Pontianak</div>
                </div>
                <!-- Repeat pattern for other work history items with dark mode classes -->
                <!-- Last item shown as example -->
                <div>
                    <div class="flex justify-between items-center mb-2">
                        <div class="text-base font-semibold dark:text-white">Kepala Diskominfo</div>
                        <div class="text-sm text-white bg-customGreen dark:bg-green-600 rounded-full px-4 py-1 inline-block text-center font-bold">2021</div>
                    </div>
                    <div class="mt-2 text-sm text-gray-500 dark:text-gray-400">Kepala Dinas Komunikasi dan Informatika Prov. Kalbar</div>
                </div>
            </div>
        </div>
        <div class="sm:w-2/3 w-full p-6">
            <!-- Nama dan jabatan untuk tampilan desktop -->
            <div class="hidden sm:block">
                <div class="text-2xl font-bold text-green-600 dark:text-green-400">SAMUEL, SE, M.Si</div>
                <div class="text-sm text-gray-600 dark:text-gray-300 mb-4">Kepala Dinas Komunikasi dan Informatika Provinsi Kalimantan Barat</div>
            </div>
            <div class="flex flex-row items-center justify-center space-x-3 mb-4 pt-24">
                <div class="flex items-center text-gray-400 dark:text-gray-300 cursor-pointer text-center" onclick="toggleVisibility('tentang');">
                    <i class="fas fa-info-circle mr-1 sm:inline-block hidden" id="icon-tentang"></i>
                    <span class="font-semibold" id="text-tentang">Tentang</span>
                </div>
                <div class="flex items-center text-gray-400 dark:text-gray-300 cursor-pointer text-center" onclick="toggleVisibility('pendidikan');">
                    <i class="fas fa-graduation-cap mr-1 sm:inline-block hidden" id="icon-pendidikan"></i>
                    <span class="font-semibold" id="text-pendidikan">Riwayat Pendidikan</span>
                </div>
                <div class="flex items-center text-gray-400 dark:text-gray-300 cursor-pointer text-center" onclick="toggleVisibility('penghargaan');">
                    <i class="fas fa-trophy mr-1 sm:inline-block hidden" id="icon-penghargaan"></i>
                    <span class="font-semibold" id="text-penghargaan">Penghargaan</span>
                </div>
            </div>
            <div class="border-t-2 border-green-600 dark:border-green-400 mb-4"></div>
            <div id="tentang" class="bg-white dark:bg-gray-800 p-6 rounded-lg shadow border-2 border-gray-300 dark:border-gray-600 h-auto">
                <div class="space-y-4">
                    <div>
                        <span class="font-semibold dark:text-white">&#8226;&nbsp; Tempat dan Tanggal Lahir:</span>
                        <div class="ml-4 dark:text-gray-300">Caong, 8 April 1966</div>
                    </div>
                    <div>
                        <span class="font-semibold dark:text-white">&#8226;&nbsp; Jenis Kelamin:</span>
                        <div class="ml-4 dark:text-gray-300"><i class="fas fa-mars"></i> Laki - Laki</div>
                    </div>
                    <div>
                        <span class="font-semibold dark:text-white">&#8226;&nbsp; Status Perkawinan:</span>
                        <div class="ml-4 dark:text-gray-300">Kawin</div>
                    </div>
                    <div>
                        <span class="font-semibold dark:text-white">&#8226;&nbsp; Pendidikan Terakhir:</span>
                        <div class="ml-4 dark:text-gray-300">S2 – Magister Ekonomi Pembangunan</div>
                    </div>
                </div>
            </div>
            <div id="pendidikan" class="bg-white dark:bg-gray-800 p-6 rounded-lg shadow border-2 border-gray-300 dark:border-gray-600 h-auto" style="display: none;">
                <div class="space-y-4">
                    <div>
                        <span class="font-semibold dark:text-white">&#8226;&nbsp; Sekolah Dasar:</span>
                        <div class="flex justify-between items-center ml-4 mt-2 mb-2">
                            <div class="text-white bg-customGreen dark:bg-green-600 rounded-full px-4 py-1 inline-block text-center" style="width: 50px; height: 30px; display: flex; align-items: center; justify-content: center;">1979</div>
                            <span class="flex-1 text-left ml-4 dark:text-gray-300">SD Subsidi Sibale Kab. Sambas</span>
                        </div>
                    </div>
                    <!-- Repeat pattern for other education items -->
                </div>
            </div>
            <div id="penghargaan" class="bg-white dark:bg-gray-800 p-6 rounded-lg shadow border-2 border-gray-300 dark:border-gray-600 h-auto" style="display: none;">
                <div class="space-y-4">
                    <div>
                        <div class="flex items-start mb-4">
                            <span class="font-semibold mr-2 dark:text-white">&#8226;</span>
                            <div class="flex-1">
                                <div class="flex justify-between items-center">
                                    <span class="dark:text-gray-300">Anugrah Parahita Ekapraya Kategori Madya Dari Menteri Pemberdayaan Perempuan Dan Perlindungan Anak</span>
                                    <span class="text-white bg-customGreen dark:bg-green-600 rounded-full px-4 py-1 inline-block text-center ml-2" style="width: 50px; height: 30px; display: flex; align-items: center; justify-content: center;">2011</span>
                                </div>
                            </div>
                        </div>
                        <!-- Repeat pattern for other awards -->
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<script>
document.addEventListener('DOMContentLoaded', function() {
    toggleVisibility('tentang');
});
function toggleVisibility(section) {
    const sections = ['tentang', 'pendidikan', 'penghargaan'];
    sections.forEach(sec => {
        document.getElementById(sec).style.display = sec === section ? 'block' : 'none';
        const iconElement = document.getElementById('icon-' + sec);
        const textElement = document.getElementById('text-' + sec);
        if (sec === section) {
            iconElement.style.color = '#03a055';
            textElement.style.color = '#03a055';
        } else {
            iconElement.style.color = 'gray';
            textElement.style.color = 'gray';
        }
        [iconElement, textElement].forEach(element => {
            element.addEventListener('mouseover', function() {
                iconElement.style.color = 'rgba(3, 160, 85, 0.5)';
                textElement.style.color = 'rgba(3, 160, 85, 0.5)';
            });
            element.addEventListener('mouseout', function() {
                iconElement.style.color = sec === section ? '#03a055' : 'gray';
                textElement.style.color = sec === section ? '#03a055' : 'gray';
            });
        });
    });
}
</script>
