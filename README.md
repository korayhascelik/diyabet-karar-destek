# 🩺 Diyabet Riski Tahmini: Yapay Zeka Destekli Klinik Karar Destek Sistemi (CDSS)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Ensemble-red.svg)
![Plotly](https://img.shields.io/badge/Plotly-Data%20Visualization-brightgreen.svg)
![CRISP-DM](https://img.shields.io/badge/Methodology-CRISP--DM-purple.svg)

Bu proje, hastaların klinik ve demografik verilerini kullanarak Tip 2 Diyabet riskini erken aşamada tespit etmeyi amaçlayan uçtan uca bir veri bilimi ve makine öğrenmesi çalışmasıdır. Çalışma, akademik ve endüstriyel standart olan **CRISP-DM** metodolojisine uygun olarak geliştirilmiştir.

## 📌 İş Anlayışı ve Tıbbi Strateji (Business Understanding)
Sağlık veri bilimi projelerinde temel amaç sadece matematiksel olarak "yüksek doğruluk (Accuracy)" elde etmek değildir. Diyabet gibi hastalıkların teşhisinde **False Negative (Hastayı gözden kaçırma)** oranı hayati risk taşır. Bu nedenle projemiz, salt Accuracy yerine **Recall (Duyarlılık)** metriğini maksimize edecek şekilde tasarlanmış ve hekimler için güvenilir bir "İkinci Görüş (Second Opinion)" algoritması olarak kurgulanmıştır.

---

## 📁 Proje Mimarisi

Sürdürülebilir bir veri akışı için klasör yapısı modüler olarak tasarlanmıştır:

```text
├── data/
│   ├── raw/                 # Orijinal Pima Indians veri seti (Müdahale edilmemiş)
│   └── processed/           # Ön işleme ve Feature Engineering sonrası temiz veri
├── figures/                 # Plotly ile üretilen etkileşimli HTML grafikler ve ekran görüntüleri
├── notebook.ipynb           # Model eğitim ve EDA süreçlerini barındıran ana dosya
└── README.md                # Proje açıklamaları
