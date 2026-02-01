# 🧬 Makine Öğrenmesi ile Alzheimer İlaç Keşfi (QSAR Modeli)

Bu proje, Alzheimer hastalığının tedavisinde kritik bir hedef olan **Asetilkolinesteraz (AChE)** enzimi üzerinde etkili olabilecek ilaç adaylarını tespit etmek amacıyla geliştirilmiş bir Yapay Zeka modelidir.

## 🚀 Proje Özeti
İlaç keşif süreçleri (Drug Discovery) oldukça maliyetli ve uzun zaman alan süreçlerdir. Bu projede, **Biyoinformatik** ve **Makine Öğrenmesi** teknikleri birleştirilerek, moleküllerin laboratuvara girmeden bilgisayar ortamında taranması ve biyolojik aktivitelerinin (**pIC50** değerlerinin) tahmin edilmesi sağlanmıştır.

## ⚙️ Nasıl Çalışır?
1.  **Veri Toplama:** ChEMBL veritabanından AChE enzimini inhibe eden binlerce molekülün verisi çekildi.
2.  **Öznitelik Çıkarımı:** Moleküllerin kimyasal formülleri (**SMILES** kodları), **RDKit** kütüphanesi kullanılarak bilgisayarın anlayabileceği sayısal verilere (Morgan Parmak İzleri) dönüştürüldü.
3.  **Model Eğitimi:** **Random Forest Regresyon** algoritması kullanılarak moleküler yapı ile biyolojik aktivite arasındaki ilişki modellendi.

## 📊 Performans ve Sonuçlar
Geliştirilen model test verileri üzerinde **0.76 R² Skoru** (%76 Başarı) elde etmiştir.
<img width="884" height="684" alt="doğruluk grafiği" src="https://github.com/user-attachments/assets/f701308d-aab8-43cd-88e2-4d41017dbb27" />


**Modelin Gerçek Hayat Testi:**
| Molekül Adı | Tür | Model Tahmini | Sonuç |
| :--- | :--- | :--- | :--- |
| **Donepezil** | Gerçek Alzheimer İlacı | **6.12 (Yüksek)** | ✅ Başarılı |
| **Paracetamol** | Ağrı Kesici (Alakasız) | **4.11 (Düşük)** | ✅ Başarılı |

Model, gerçek ilaçları (Donepezil) potansiyel olmayan moleküllerden (Paracetamol) başarıyla ayırt edebilmektedir.

## 🛠️ Kullanılan Teknolojiler
* **Python** (Programlama Dili)
* **RDKit** (Biyoinformatik / Moleküler Modelleme)
* **Scikit-learn** (Makine Öğrenmesi Algoritmaları)
* **Pandas & NumPy** (Veri Analizi)

