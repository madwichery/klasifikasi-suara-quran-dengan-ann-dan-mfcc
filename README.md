# klasifikasi-suara-quran-dengan-ann-dan-mfcc
Mengidentifikasi suara Al-Qur'an yang dibacakan sesuai dengan surat dan ayatnya. Menggunakan skema MLOps (Machine Learning Operations) dengan library Weight and Biases (WANDB).

Data terdapat di Artifact Wandb, dipreprocessing ke MFCC kemudian diklasifikasikan dengan ANN.

flow:
1. [Data yang digunakan diupload ke Artifact Weights & Biases](https://wandb.ai/madwichery/skripsi-madwichery-klasifikasi-32-ayat-quran-EDA/artifacts/dataset/raw-dataset/v0/files)
2. [Explanatory Data Analysis: data audio memiliki variabilitas panjang yang berbeda-beda tiap ayat.](https://wandb.ai/madwichery/skripsi-madwichery-klasifikasi-32-ayat-quran-EDA/reports/Exploratory-Data-Analysis-Skripsi-Menghadapi-Variabilitas-Durasi-Audio-dalam-Tugas-Klasifikasi--VmlldzozODI2NzUx) 
3. [Preprocessing data audio](https://gist.github.com/madwichery/e41b08507672980d9b694b3e7c612ba8)
4. [Training](https://gist.github.com/madwichery/53e27a4a0130fec29682487e34f97578)

![](/img/3 Best Epoch v f1_score.png) 
- 3 Arsitektur sebagai skenario percobaan, mencari parameter yang bisa ditraining lebih lanjut dengan parameter yang tidak overfit dengan nilai f1 tiap arsitektur mengalami kenaikan sebesar yaitu 43,1%, 46%, dan 46,4%.

![](/img/3 Confusion Matrix.png) 
- Hasil Klasifikasi terbaik dari ketiga parameter Arsitektur ketiga di atas.
