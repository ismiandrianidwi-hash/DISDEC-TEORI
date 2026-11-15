# Materi Minggu 1: Pengenalan Sistem Terdistribusi dan Terdesentralisasi

Prompt: Pahami secara menyeluruh modul ini, Baik, sekarang bantu saya buatkan ringkasan dari keseluruhan materi pada modul ini. <br>

Bagian yang disesuaikan dari keluaran prompt ada pada: 

### 1. Arti Penting Sistem Terdistribusi dan Terdesentralisasi

Sistem terdistribusi dan terdesentralisasi merupakan bagian penting dalam perkembangan teknologi modern. Kedua sistem ini dibutuhkan karena pertumbuhan jumlah data dan pengguna semakin besar. Layanan modern memerlukan skalabilitas, performa tinggi, ketersediaan 24/7, serta kemampuan untuk tetap beroperasi ketika terjadi kegagalan pada sebagian komponennya (fault tolerance). <br>

Bagian ini saya tambahkan dari diri sendiri : <br>

Istilah penting: <br>

- Skalabilitas : kemampuan sistem untuk berkembang dan menangani peningkatan beban kerja tanpa menurunkan kinerja.
- Fault Tolerance: kemampuan sistem untuk tetap beroperasi meskipun sebagian perangkat keras atau perangkat lunak mengalami kegagalan.

### 2. Pengertian Sistem Terdistribusi

Sistem terdistribusi adalah kumpulan komputer independen yang saling berkomunikasi melalui jaringan dan terlihat oleh pengguna sebagai satu sistem yang utuh. <br>

Karakteristik dasarnya meliputi:<br>

- Komponen komputer bekerja secara independen.
- Komunikasi dilakukan melalui jaringan.
- Memiliki transparansi lokasi, akses, replikasi, dan kegagalan.

Bagian contoh saya tambahkan dari diri sendiri : <br>

Contoh: Google, Netflix, YouTube, dan Instagram.

### 3. Arsitektur Sistem Dasar

Terdapat tiga jenis arsitektur dasar sistem terdistribusi: <br>

- Client-Server: client meminta layanan, sedangkan server menyediakan layanan atau sumber daya.
- Peer-to-Peer (P2P): setiap komputer atau node dapat saling berbagi sumber daya dan berkomunikasi secara langsung.
- Hybrid: gabungan arsitektur Client-Server dan Peer-to-Peer.

### 4. Karakteristik Sistem Terdistribusi

Sistem terdistribusi memiliki lima karakteristik utama:<br>

- Transparansi lokasi: pengguna tidak perlu mengetahui lokasi sumber daya.
- Skalabilitas: sistem dapat dikembangkan sesuai peningkatan kebutuhan.
- Fault tolerance: sistem tetap berfungsi ketika terjadi kegagalan komponen.
- Kinerja tinggi: mampu menangani permintaan dan pekerjaan dengan baik.
- Heterogenitas: dapat menggunakan perangkat keras, perangkat lunak, dan jaringan yang berbeda.

### 5. Pengertian Sistem Terdesentralisasi

Sistem terdesentralisasi adalah sistem yang kendali dan pengambilan keputusannya dibagikan kepada beberapa pihak atau node, bukan hanya bergantung pada satu pusat kontrol.<br>

Terdapat dua konsep: <br>

- Sentralisasi: seluruh kendali berada pada satu titik pusat.
- Desentralisasi: kendali dibagikan kepada beberapa pihak.

Keputusan dalam sistem terdesentralisasi dapat dilakukan melalui mekanisme konsensus, yaitu proses mencapai kesepakatan antar-node. <br>

Bagian ini saya tambahkan dari diri sendiri : <br>

Contohnya adalah Blockchain, DNS, dan BitTorrent. 

###  6. Perbedaan Sistem Terdistribusi dan Terdesentralisasi

Kedua sistem memiliki hubungan, tetapi berbeda dalam fokus penerapannya. <br>

- Sistem terdistribusi: berfokus pada pembagian beban kerja ke beberapa komputer.
- Sistem terdesentralisasi: berfokus pada pembagian kendali atau pengambilan keputusan.

Contoh sistem terdistribusi adalah Google File System dan MinIO, sedangkan contoh sistem terdesentralisasi adalah Blockchain.

### 7. Studi Kasus Sistem Terdistribusi

Sistem terdistribusi telah diterapkan dalam berbagai teknologi, terutama untuk mengelola data dan melayani banyak pengguna.<br>

Contohnya:<br>

- Google File System (GFS) dan HDFS: digunakan untuk penyimpanan data berukuran besar.
- Apache Kafka dan Apache Pulsar: digunakan untuk messaging dan streaming data.
- Netflix dan Twitch: menyediakan layanan streaming.
- YouTube: menyediakan layanan berbagi dan menonton video.
- Instagram, Threads, Facebook, dan TikTok: menyediakan layanan media sosial.

### 8. Studi Kasus Sistem Terdesentralisasi

Beberapa contoh penerapan sistem terdesentralisasi adalah:<br>

- Blockchain: teknologi penyimpanan transaksi dalam blok yang saling terhubung dan menggunakan mekanisme konsensus. Contohnya Bitcoin dan Ethereum.
- DNS (Domain Name System): sistem yang membantu menerjemahkan nama domain menjadi alamat IP.
- BitTorrent: teknologi berbagi file melalui jaringan Peer-to-Peer.

### 9. CAP Theorem

CAP Theorem atau Brewer's Theorem diperkenalkan oleh Eric Brewer pada tahun 2000. Teorema ini menjelaskan tiga konsep penting dalam sistem penyimpanan data terdistribusi.

1. Consistency: setiap operasi pembacaan memberikan data hasil penulisan terbaru atau menghasilkan error.
2. Availability: setiap permintaan pada node yang tidak mengalami kegagalan akan mendapatkan respons yang tidak error, meskipun datanya belum terbaru.
3. Partition Tolerance: sistem tetap dapat beroperasi meskipun komunikasi antar-node mengalami gangguan atau terputus.

Ketika terjadi network partition, sistem harus menentukan prioritas antara AP dan CP. <br>

Arti ap dan cp ini dari diri saya sendiri : <br>

1. AP (Availability + Partition Tolerance): mengutamakan ketersediaan layanan dan toleransi gangguan jaringan, tetapi data berisiko belum sinkron. Contoh dalam modul: MongoDB.
2. CP (Consistency + Partition Tolerance): mengutamakan konsistensi data dan toleransi gangguan jaringan, tetapi beberapa permintaan dapat ditolak. Contoh dalam modul: Apache Cassandra.

### 10. Konsistensi Data

Konsistensi data merupakan kondisi yang berkaitan dengan kesesuaian data ketika disimpan dan diakses oleh pengguna. <br>

Terdapat dua jenis konsistensi:<br>

- Strong Consistency: hasil pembacaan data selalu mencerminkan penulisan terbaru. Contohnya sistem perbankan.
- Eventual Consistency: data mungkin belum langsung sama pada seluruh bagian sistem, tetapi akan menjadi konsisten setelah beberapa waktu. Contohnya media sosial.

### 11. Tantangan Sistem Terdistribusi dan Terdesentralisasi

Dalam penerapannya, terdapat beberapa tantangan yang perlu diperhatikan:<br>

1. Latency: waktu yang dibutuhkan untuk memproses permintaan atau memberikan respons.
2. Throughput: jumlah pekerjaan atau permintaan yang dapat diproses dalam periode tertentu.
3. Keamanan: sistem dapat menghadapi serangan seperti DDoS dan Sybil Attack.
4. Kompleksitas manajemen node: semakin banyak node, semakin sulit pengelolaan dan pemantauannya.
5. Governance: berkaitan dengan tata kelola dan pengambilan keputusan dalam sistem terdesentralisasi. <br>

Sybil Attack merupakan serangan yang dilakukan dengan membuat banyak identitas palsu untuk memanipulasi pengaruh, suara, atau reputasi dalam jaringan.

### 12. Tren Masa Depan

Perkembangan sistem terdistribusi dan terdesentralisasi terus mengalami kemajuan. Beberapa tren yang dibahas dalam modul adalah:<br>

- Cloud-native: pengembangan aplikasi berbasis cloud dengan teknologi seperti Docker dan Kubernetes.
- Edge & Fog Computing: pemrosesan data dilakukan lebih dekat dengan sumber data atau perangkat pengguna.
- Web3 & DeFi: perkembangan layanan internet dan keuangan berbasis teknologi terdesentralisasi.
- Federated Data-Learning: pendekatan pembelajaran AI terdistribusi yang memungkinkan pelatihan dilakukan di beberapa perangkat atau lokasi.

### 13. Kesimpulan

Sistem terdistribusi dan terdesentralisasi merupakan fondasi penting dalam perkembangan teknologi modern. Sistem terdistribusi berfokus pada pembagian beban kerja ke beberapa komputer untuk meningkatkan kinerja, skalabilitas, dan ketersediaan layanan. Sementara itu, sistem terdesentralisasi berfokus pada pembagian kendali dan pengambilan keputusan agar tidak bergantung pada satu pusat kontrol. <br>

Keduanya memiliki karakteristik, arsitektur, dan penerapan yang berbeda, tetapi saling berkaitan. Dalam penerapannya, terdapat berbagai tantangan seperti keamanan, konsistensi data, latency, throughput, dan pengelolaan node. Perkembangan teknologi seperti Cloud-native, Edge Computing, Web3, dan Federated Learning menunjukkan bahwa kedua sistem tersebut akan terus menjadi bagian penting dari perkembangan teknologi di masa depan.