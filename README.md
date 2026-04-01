# Transjakarta BRT Operational & Network Analysis
An in-depth analysis of the Transjakarta Bus Rapid Transit (BRT) network using GTFS (General Transit Feed Specification) data standards. This project leverages Graph Theory to evaluate route efficiency, stop connectivity, and network robustness against operational disruptions.

*This project serves as a big data analytics case study integrating spatial data processing with network science metrics to optimize public transportation systems.*

## 📝 Project Description
This project constructs a graph representation of the Transjakarta operational system, where bus stops function as nodes and bus trips as edges. By analyzing this network structure, we can identify crucial hubs within Jakarta's transit system and measure how efficiently passengers can navigate from one point to another.

## ✨ Key Features
- **GTFS Data Integration**: Processing core GTFS components including `stops.txt`, `stop_times.txt`, `trips.txt`, and `routes.txt` into a unified data structure.
- **Network Graph Construction**: Building directed graphs representing connections between stops based on actual bus trip schedules.
- **Centrality Metrics Analysis**: Identifying the most influential stops using *Degree Centrality*, *Closeness Centrality*, and *Betweenness Centrality*.
- **Efficiency & Robustness Evaluation**: Calculating global network efficiency and simulating the impact of critical node removal on system flow.
- **Corridor Metadata Mapping**: Integrating corridor names to provide operational context to the technical analysis.

## 🛠️ Tech Stack & Implementation
- **Programming Language**: Python 3.x
- **Network Science**: NetworkX (for graph modeling and centrality metric calculations).
- **Data Manipulation**: Pandas (for GTFS data cleaning and transformation).
- **Environment**: Google Colab.

## 📊 Methodology
- **Data Logic**: Utilizing `stops` as nodes and `stop_times` to establish relationships based on trip sequences.
- **Graph Modeling**: Implementing `DiGraph` (Directed Graph) to reflect specific bus travel directions.
- **Critical Node Analysis**: Measuring which stops most frequently act as bridges between different routes (high betweenness), representing potential bottlenecks.

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
- **Environment**: Google Colab.

## 📊 Methodology
- **Data Logic**: Menggunakan `stops` sebagai titik pemberhentian dan `stop_times` sebagai pembentuk relasi antar titik berdasarkan urutan perjalanan.
- **Graph Modeling**: Implementasi graf menggunakan `DiGraph` (Directed Graph) untuk mencerminkan arah perjalanan bus yang spesifik.
- **Critical Node Analysis**: Mengukur halte mana yang paling sering menjadi jembatan antar rute berbeda (high betweenness), yang berpotensi menjadi titik kemacetan jika terjadi gangguan.

## ⚙️ Installation & Usage
- **Data Prep**: Pastikan file standar GTFS (`stops.txt`, `stop_times.txt`, dll) tersedia di direktori kerja.
- **Requirements**: Instalasi pustaka melalui `pip install pandas networkx`.
- **Execution**: Jalankan notebook untuk melihat hasil analisis efisiensi jaringan secara otomatis.
