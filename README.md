# 📚 FastText & SciBERT Tabanlı Akademik Makale Öneri Sistemi

## 📌 Proje Açıklaması

Bu proje, anahtar kelime tabanlı doküman benzerliği kullanarak araştırma makaleleri için bir öneri sistemi geliştirmeyi amaçlamaktadır.

Model, kullanıcı girdisine göre benzer makaleleri tespit etmek için aşağıdaki yöntemleri kullanır:

- 🔎 **FastText**
- 🧠 **SciBERT**
- 📐 **Cosine Similarity**
- 🧹 **NLP ön işleme teknikleri**

---

## 🎯 Proje Amacı

Bu sistem:

- Kullanıcının girdiği metne göre benzer akademik makaleleri önerir.
- Anahtar kelime çıkarımı yapar.
- Dokümanlar arası semantik benzerliği hesaplar.
- Dinamik kullanıcı profili oluşturarak öneri kalitesini artırır.

---

## 🛠 Kullanılan Teknolojiler

- Python
- FastText
- SciBERT (HuggingFace Transformers)
- Scikit-learn
- NumPy
- Pandas

---

## 📂 Veri Setleri

Projede aşağıdaki akademik veri setleri kullanılmıştır:

- **Inspec Dataset**
- **Krapivin2009 Dataset**

Bu veri setleri, anahtar kelime çıkarımı ve doküman benzerliği için kullanılmıştır.

---

## ⚙️ Sistem Mimarisi

### 1️⃣ Veri Ön İşleme

- Küçük harfe çevirme
- Noktalama temizleme
- Stopword çıkarımı
- Tokenization

### 2️⃣ Vektörleştirme

- FastText ile kelime embedding
- SciBERT ile doküman embedding

### 3️⃣ Benzerlik Hesaplama

- Cosine Similarity kullanılarak benzerlik skoru hesaplanır.

### 4️⃣ Öneri Motoru

- Kullanıcı girdisine en yakın makaleler sıralanır.
- Precision ve Recall ile performans değerlendirmesi yapılır.

---

## 📊 Model Değerlendirme

Model performansı aşağıdaki metrikler ile ölçülmektedir:

- Precision
- Recall
- Cosine Similarity Score

---

## ▶️ Kurulum

Projeyi lokal ortamda çalıştırmak için aşağıdaki adımları takip edin.

```bash
# 1️⃣ Repository'yi klonlayın
git clone https://github.com/kullaniciadi/repo-adi.git

# 2️⃣ Proje klasörüne girin
cd repo-adi

# 3️⃣ (Opsiyonel) Sanal ortam oluşturun
python -m venv venv

# 4️⃣ Sanal ortamı aktifleştirin
# Windows:
venv\Scripts\activate
# MacOS / Linux:
source venv/bin/activate

# 5️⃣ Gerekli paketleri yükleyin
pip install -r requirements.txt

# 6️⃣ Projeyi çalıştırın
python main.py
```

