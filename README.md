## Amazon app Text classification
Proyek ini merupakan sentiment analysis dari review applikasi Amazon di AppStore. 
Tujuannya untuk memprediksi sentiment dari review yang diberikan user kedalam 5 kelas yaitu VERY NEGATIVE, NEGATIVE, NEUTRAL, POSITIVE, VERY POSITIVE, dan jika diartikan dalam 3 kelas
VERY NEGATIVE, NEGATIVE -> NEGATIVE
NEUTRAL -> NEUTRAL
POSITIVE, VERY POSITIVE -> POSITIVE

### Data

Data diperoleh dari hasil scrap review Amazon di AppStore dengan 10000 dataset

### Problem

1. Pelabelan dilakukan dengan menggunakan pretrained model bert dari transformer dan sama sekali tidak melakukan pelabelan dari data rating review aplikasi
2. Distribusi data yang imbalance menyebabkan overfitting dan akurasi validasi tidak meningkat, solusinya dilakukan oversampling data sehinga data mengingkat menjadi 30 ribu lebih dan distribusi data menjadi  seimbang untuk masing-masing kelas
Algoritm

### Model
Algoritma yang digunakan adalah SVM, LSTM, dan GRU

### Result

Hasil dari algoritma yang digunakan adalah sebagai berikut
SVM = 96%
LSTM = 97%
GRU = 97%
