---
author: Katheryn Fox
title: FAQ
date: 2025-01-04T12:56:00
---

<div style="font-family: 'Poppins', sans-serif;">

<script>
const faqData = [
    {
        question: "Apa yang dimaksud dengan informasi publik?",
        answer: "Informasi publik adalah informasi yang dihasilkan, disimpan, dikelola dan dikirim oleh organisasi Badan Publik yang berkaitan dengan penyelenggara dan penyelenggaraan informasi organisasi Badan Publik dan/atau penyelenggaraan badan publik lainnya dalam kerangka koordinasi pengelolaan dan pelayanan informasi lain yang berkaitan dengan kepentingan publik."
    },
    {
        question: "Berapa lama waktu yang dibutuhkan untuk mendapatkan informasi publik?", 
        answer: "Informasi akan diberikan paling lama dalam waktu 10 (sepuluh) hari kerja dan dapat diperpanjang paling lambat 7 (tujuh) hari kerja berikutnya dengan memberikan alasan secara tertulis."
    },
    {
        question: "Siapa saja yang boleh meminta informasi publik?",
        answer: "Siapa saja boleh meminta informasi publik, baik perseorangan maupun badan hukum dengan menyertakan fotokopi identitas dan fotokopi akta badan hukum untuk pemohon dari badan hukum."
    }
];

document.addEventListener('DOMContentLoaded', function() {
    const faqContainer = document.getElementById('faq-container');
    
    faqData.forEach((item, index) => {
        const faqItem = document.createElement('div');
        faqItem.className = 'faq-item mb-4';
        faqItem.innerHTML = `
            <div class="faq-question rounded-xl bg-white border border-gray-300 p-4 cursor-pointer flex justify-between items-center relative" onclick="toggleAnswer(${index})">
                <div class="green-line"></div>
                <span class="font-semibold">${item.question}</span>
                <div class="toggle-icon w-6 h-6 bg-customGreen rounded-full flex items-center justify-center text-white flex-shrink-0">
                    <span class="plus-icon">+</span>
                </div>
            </div>
            <div class="faq-answer bg-customGreen p-4 rounded-b-lg mt-0 hidden text-white">
                ${item.answer}
            </div>
        `;
        faqContainer.appendChild(faqItem);
    });
});

function toggleAnswer(index) {
    const answers = document.querySelectorAll('.faq-answer');
    const icons = document.querySelectorAll('.plus-icon');
    
    answers[index].classList.toggle('hidden');
    icons[index].style.transform = answers[index].classList.contains('hidden') ? 'rotate(0deg)' : 'rotate(45deg)';
}
</script>

<style>
.faq-question {
    transition: background-color 0.3s ease;
}

.faq-question:hover {
    background-color: #f8f8f8;
}

.plus-icon {
    transition: transform 0.3s ease;
    font-size: 20px;
    line-height: 1;
}

.faq-answer {
    transition: all 0.3s ease;
}

.green-line {
    position: absolute;
    left: 0;
    top: 0;
    bottom: 0;
    width: 8px;
    background-color: #10B981;
    border-top-left-radius: 1.25rem;
    border-bottom-left-radius: 1.25rem;
}
</style>

<div id="faq-container" class="max-w-3xl mx-auto py-8">
</div>

</div>
