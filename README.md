# Aspect Based Sentiment Analysis (ABSA) Terhadap Isu Cyberbullying pada Komentar Instagram

## Project Overview
Proyek ini bertujuan untuk menganalisis komentar Instagram terkait isu cyberbullying menggunakan Aspect-Based Sentiment Analysis (ABSA) dengan model IBM Granite 3.1-8b-instruct. Dengan fokus pada klasifikasi sentimen (bullying/non-bullying) dan ekstraksi aspek spesifik, proyek ini mengatasi tantangan pelecehan online yang memengaruhi kesehatan mental pengguna, terutama di Indonesia dengan prevalensi hingga 49%. Pendekatan ini memberikan wawasan multi-dimensi untuk mitigasi cyberbullying dan pengembangan kebijakan platform digital.

## Raw Dataset Link
- [DATASET CYBERBULLYING INSTAGRAM - FINAL.xlsx](https://www.kaggle.com/code/syauqiddjohan/skripsi-sentiment-analysis-project/input)
- [stopwordsID.csv](https://www.kaggle.com/code/syauqiddjohan/skripsi-sentiment-analysis-project/input)
- [kamus_singkatan.csv](https://www.kaggle.com/code/syauqiddjohan/skripsi-sentiment-analysis-project/input)

## Insight & Findings
- Model mencapai akurasi rata-rata ~0.7 dalam klasifikasi sentimen, menunjukkan performa sedang karena keterbatasan few-shot learning pada teks informal Instagram.
- Aspek dominan dalam bullying meliputi "penampilan" dan "perilaku", dengan distribusi komentar bullying sekitar 37% dari dataset.
- Preprocessing efektif dalam normalisasi teks, tetapi penghapusan stopwords dapat mengurangi konteks sentimen; variasi parameter (top_k, top_p) memiliki dampak minimal pada peningkatan akurasi.
- Wordcloud mengungkap kata kunci seperti "muka" dan "jelek" pada komentar bullying, sementara "keren" dan "cantik" dominan pada non-bullying.

## AI Support Explanation
IBM Granite 3.1-8b-instruct diimplementasikan melalui Replicate API untuk few-shot learning, memungkinkan klasifikasi sentimen dan ekstraksi aspek tanpa pelatihan ulang. Google Colab digunakan sebagai platform untuk preprocessing, inferensi, dan evaluasi, dengan integrasi pustaka seperti langchain_community dan scikit-learn untuk tuning parameter dan metrik performa.
