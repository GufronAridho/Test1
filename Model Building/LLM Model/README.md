## Overview
README ini akan menjelaskan pembangunan model LLM dari HuggingFace yaitu BERT.
# Lets Build

## Dataset and Algorithm

### 1. Dataset
- Data Collection <br />
Kami menemukan data pertanyaan kami dari berbagai situs yang memuat pembahasan mengenai gempa, beberapa situsnya adalah sebagai berikut: <br />
https://www.usgs.gov/programs/earthquake-hazards/faqs-category <br />
https://www.earthquakescanada.nrcan.gc.ca/info-gen/faq-en.php <br />
https://scweb.cwa.gov.tw/en-us/guidance/faq <br />
https://www.earthquakes.bgs.ac.uk/education/faqs/faq_index.html <br />
https://polarisdrt.org/100-frequently-asked-questions-about-earthquakes-and-their-answers/ <br />
https://www.bmkg.go.id/ <br />
https://id.quora.com/

- Data Cleaning <br />
Data Cleaning yang kami lakukan dibuat secara mmanual, dengan point pemilihan seperti :
> "Apakah pertanyaan tersebut relate ke wilayah Indonesia ?" <br />
> "Apakah pertanyaan tersebut berguna ?"

- Data Transformation <br />
Data daari pertanyaan dan jawaban yang telah didapat diubah menjadi format .json dengan struktur seperti berikut :
```
{
    "intents": [
        {
            "tag": "",
            "patterns": [
                ""
            ],
            "responses": [
                ""
            ],
            "context": [
                ""
            ]
        },
        {
            "tag": "",
            "patterns": [
                ""
            ],
            "responses": [
                ""
            ],
            "context": [
                ""
            ]
        }
    ]
}
```

Contoh 
```
{
    "intents": [
        {
            "tag": "intensitas",
            "patterns": [
                "Apa itu intensitas gempa bumi?",
                "Bisakah Anda menjelaskan tentang intensitas gempa?",
                "Bagaimana definisi intensitas dalam konteks gempa bumi?",
                "Apa yang dimaksud dengan intensitas gempa bumi?",
            ],
            "responses": [
                "Intensitas gempa bumi adalah ukuran kualitatif kekuatan gempa di suatu tempat yang ditentukan berdasarkan kerusakan dan hasil pengamatan efek gempa bumi di lokasi tersebut, yang dihitung berdasarkan pengamatan subjektif. Intensitas gempa bumi menunjukkan dampak yang dirasakan di permukaan bumi dan dapat berbeda dengan magnitudo gempa, yang menunjukkan kekuatan energi yang dihasilkan oleh gempa. Skala yang digunakan untuk mengukur intensitas gempa adalah Skala MMI (Modified Mercalli Intensity) yang dicetuskan oleh Giuseppe Mercalli pada tahun 1902. Namun, Indonesia memiliki skala intensitasnya sendiri yaitu Skala Intensitas Gempa Bumi (SIG) yang digunakan oleh BMKG."
            ],
            "context": [
                ""
            ]
        },
        {
            "tag": "peran_yang_bisa_dilakukan",
            "patterns": [
                "Apa yang bisa saya lakukan untuk korban pasca gempa",
                "Apa yang bisa saya lakukan untuk membantu korban pasca gempa?",
                "Bagaimana saya dapat memberikan kontribusi kepada korban gempa?",
                "Apakah ada cara bagi saya untuk membantu meringankan beban korban pasca gempa?",
            ],
            "responses": [
                "Ada beberapa peran yang bisa Anda lakukan untuk membantu korban pasca gempa. Salah satunya adalah dengan memberikan donasi kepada lembaga yang terpercaya. Donasi ini dapat digunakan untuk meringankan beban korban dalam hal material seperti perlengkapan hidup sehari-hari, tempat tinggal darurat, dan perawatan kesehatan. Selain itu, Anda juga bisa menjadi relawan untuk membantu pemerintah atau organisasi kemanusiaan dalam menangani pengungsian korban gempa. Dengan bergabung sebagai relawan, Anda dapat memberikan bantuan langsung kepada korban seperti pendistribusian bantuan, merawat anak-anak atau lansia, serta membantu dalam proses pemulihan dan rekonstruksi. Setiap kontribusi Anda, baik dalam bentuk donasi maupun menjadi relawan, sangat berarti bagi mereka yang terdampak gempa."
            ],
            "context": [
                ""
            ]
        }
    ]
}
```

### 2. Algorithm

- Framework <br />
Kami menggunakan TensorFlow dan Keras.

- Pembangunan Model <br />
Masukkan kode training dan juga spesifikasi model, seperti epoch, learning rate, batch size, dan lain sebagainya.

- Model Evaluation <br />
Masukkan metrik evaluasi model seperti accuracy, precision, recall, F1-score, dan lain - lain.

## Prototype
Disesuaikan dengan kebutuhan atau bisa ditiru dari laporan dokumentasi massive.

## Integration
Disesuaikan dengan kebutuhan atau bisa ditiru dari laporan dokumentasi massive.

## Deployment
Disesuaikan dengan kebutuhan atau bisa ditiru dari laporan dokumentasi massive.

## Result
Disesuaikan dengan kebutuhan atau bisa ditiru dari laporan dokumentasi massive.

## Conclusion
Disesuaikan dengan kebutuhan atau bisa ditiru dari laporan dokumentasi massive.
