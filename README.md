# Transjakarta BRT Operational & Network Analysis
An in-depth analysis of the Transjakarta Bus Rapid Transit (BRT) network using GTFS (General Transit Feed Specification) data standards. This project leverages Graph Theory to evaluate route efficiency, stop connectivity, and network robustness against operational disruptions.

*This project serves as a big data analytics case study integrating spatial data processing with network science metrics to optimize public transportation systems.*

## 📝 Project Description
This project constructs a graph representation of the Transjakarta operational system, where bus stops function as nodes and bus trips as edges. By analyzing this network structure, we can identify crucial hubs within Jakarta's transit system and measure how efficiently passengers can navigate from one point to another.

## 📂 Project Structure

```text
├── data/               # GTFS source files (.txt)
├── notebooks/          # Analysis & Graph modeling (.ipynb)
├── .gitignore          # Files to exclude from Git
├── README.md           # Documentation
└── requirements.txt    # Required libraries
```

## ✨ Key Features
- **GTFS Data Integration**: Processing core GTFS components including `stops.txt`, `stop_times.txt`, `trips.txt`, and `routes.txt` into a unified data structure.
- **Network Graph Construction**: Building directed graphs representing connections between stops based on actual bus trip schedules.
- **Centrality Metrics Analysis**: Identifying the most influential stops using *Degree Centrality*, *Closeness Centrality*, and *Betweenness Centrality*.
- **Efficiency & Robustness Evaluation**: Calculating global network efficiency and simulating the impact of critical node removal on system flow.
- **Corridor Metadata Mapping**: Integrating corridor names to provide operational context to the technical analysis.

## 🛠️ Tech Stack
- **Language**: Python 3.x
- **Network Science**: NetworkX
- **Data Manipulation**: Pandas
- **Environment**: Google Colab / Local Jupyter

## 📊 Methodology
- **Data Logic**: Utilizing `stops` as nodes and `stop_times` to establish relationships based on trip sequences.
- **Graph Modeling**: Implementing `DiGraph` (Directed Graph) to reflect specific bus travel directions.
- **Critical Node Analysis**: Measuring which stops most frequently act as bridges between different routes (high betweenness), representing potential bottlenecks.

## ⚙️ Installation & Usage

### 1. Prerequisites

Ensure you have the following GTFS files in your `data/` directory:

  - `stops.txt`, `stop_times.txt`, `trips.txt`, `routes.txt`

### 2. Setup Environment

```bash
# Clone the repository
git clone https://github.com/Billy1205/transjakarta-network-analysis.git
cd transjakarta-network-analysis

# Install dependencies
pip install -r requirements.txt
```

### 3. Running the Analysis

1.  Open the notebook in the `notebooks/` folder.
2.  Ensure the file paths to the GTFS `.txt` files are correctly pointed to the `data/` folder.
3.  Run all cells to generate centrality rankings and efficiency visualizations.

***

# Transjakarta BRT Operational & Network Analysis
Analisis mendalam terhadap jaringan transportasi Bus Rapid Transit (BRT) Transjakarta menggunakan standar data GTFS (*General Transit Feed Specification*). Proyek ini memanfaatkan teori graf untuk mengevaluasi efisiensi rute, konektivitas halte, dan ketahanan jaringan terhadap gangguan operasional.

*Proyek ini merupakan studi kasus analitik data besar yang mengintegrasikan pemrosesan data spasial dengan metrik network science untuk mengoptimalkan sistem transportasi publik.*

## 📝 Project Description
Proyek ini membangun representasi graf dari sistem operasional Transjakarta, di mana setiap halte berfungsi sebagai *node* dan perjalanan bus sebagai *edge*. Dengan menganalisis struktur jaringan ini, kita dapat mengidentifikasi titik-titik krusial (hub) dalam sistem transportasi Jakarta dan mengukur seberapa efisien penumpang dapat berpindah dari satu titik ke titik lainnya.

## ✨ Key Features
- **GTFS Data Integration**: Mengolah komponen utama GTFS termasuk `stops.txt`, `stop_times.txt`, `trips.txt`, dan `routes.txt` menjadi struktur data yang terpadu.
- **Network Graph Construction**: Membangun graf berarah yang merepresentasikan koneksi antar halte berdasarkan jadwal perjalanan bus yang sebenarnya.
- **Centrality Metrics Analysis**: Mengidentifikasi halte paling berpengaruh menggunakan *Degree Centrality*, *Closeness Centrality*, dan *Betweenness Centrality*.
- **Efficiency & Robustness Evaluation**: Menghitung efisiensi global jaringan dan melakukan simulasi dampak penghapusan *node* kritikal terhadap kelancaran sistem.
- **Corridor Metadata Mapping**: Integrasi nama koridor untuk memberikan konteks operasional pada hasil analisis teknis.

## 🛠️ Tech Stack & Implementation
- **Programming Language**: Python 3.x
- **Network Science**: NetworkX (untuk pemodelan graf dan perhitungan metrik sentralitas).
- **Data Manipulation**: Pandas (untuk pembersihan dan transformasi data GTFS).

## 📊 Methodology
- **Data Logic**: Menggunakan `stops` sebagai titik pemberhentian dan `stop_times` sebagai pembentuk relasi antar titik berdasarkan urutan perjalanan.
- **Graph Modeling**: Implementasi graf menggunakan `DiGraph` (Directed Graph) untuk mencerminkan arah perjalanan bus yang spesifik.
- **Critical Node Analysis**: Mengukur halte mana yang paling sering menjadi jembatan antar rute berbeda (high betweenness), yang berpotensi menjadi titik kemacetan jika terjadi gangguan.

## ⚙️ Instalasi & Penggunaan

### 1. Prasyarat
Pastikan file standar GTFS berikut tersedia di folder `data/`:
`stops.txt`, `stop_times.txt`, `trips.txt`, dan `routes.txt`.

### 2. Persiapan Lingkungan

```bash
# Klon repositori
git clone https://github.com/Billy1205/transjakarta-network-analysis.git
cd transjakarta-network-analysis

# Instal pustaka yang diperlukan
pip install -r requirements.txt
```

### 3. Menjalankan Analisis

1.  Buka notebook di dalam folder `notebooks/`.
2.  Pastikan jalur file (path) ke data GTFS sudah benar.
3.  Jalankan semua sel untuk melihat skor sentralitas halte dan efisiensi jaringan.
