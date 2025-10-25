# Math for Technical Interviews

## Seberapa banyak matematika yang perlu saya kuasai untuk wawancara teknis?

Jawaban singkatnya: cukup matematika setingkat SMA.

Ilmu komputer sering dikaitkan dengan matematika, dan di beberapa universitas bahkan jurusan ilmu komputer berada di bawah fakultas matematika. Namun, pada kenyataannya, sebagian besar wawancara untuk posisi software engineer dan pekerjaan sehari-hari di bidang rekayasa perangkat lunak hanya memerlukan matematika dasar setingkat SMA.

## Tapi saya pernah melihat soal di LeetCode yang butuh trik matematika rumit!

LeetCode memiliki lebih dari 2000 soal, sebagian besar dikirimkan oleh pengguna. Jadi, keberadaan satu soal yang melibatkan trik matematika tertentu di antara ribuan soal tidak terlalu berarti. Yang penting adalah apakah soal semacam itu benar-benar muncul dalam wawancara sesungguhnya. Jika melihat daftar soal yang paling sering ditanyakan perusahaan besar, soal yang membutuhkan trik atau rumus matematika tingkat lanjut sangat jarang muncul. Soal yang mengandalkan pengetahuan matematika khusus lebih bersifat knowledge test, sedangkan wawancara teknis dirancang untuk menguji kemampuan coding dan problem-solving, bukan hafalan rumus matematika.

## Bagaimana kalau saya sial dan dapat soal matematika yang susah?

Di kebanyakan perusahaan, hasil penilaian kandidat ditinjau ulang oleh insinyur lain di luar pewawancara. Jika sebuah pertanyaan dianggap terlalu sulit atau tidak relevan, maka sesi tersebut akan diberi bobot lebih kecil dalam keputusan akhir. Jadi, tidak perlu terlalu khawatir jika Anda tidak menguasai matematika lanjutan.

## Memahami Sistem Bilangan (Number Bases)

Sebelum masuk ke konsep logaritma, penting untuk memahami konsep “basis” dalam matematika. Basis menentukan jumlah digit unik dan nilai yang diwakili oleh setiap posisi dalam suatu sistem bilangan.

### Basis 10 (Desimal):

Manusia secara alami menggunakan sistem desimal (basis 10) dengan sepuluh digit unik: 0 hingga 9. Polanya sederhana — setelah mencapai angka 9, kita menambah satu digit di depan dan mulai lagi dari 10. Setiap posisi digit ke kiri mewakili pangkat 10 yang lebih tinggi.

Contoh pada angka 352:

- Digit 2 berada di posisi satuan (10⁰)
- Digit 5 berada di posisi puluhan (10¹)
- Digit 3 berada di posisi ratusan (10²)

### Transisi ke Basis 2 dalam Ilmu Komputer:

Sebaliknya, komputer beroperasi menggunakan sistem biner (basis 2), yang hanya memiliki dua digit unik: 0 dan 1. Hal ini disebabkan oleh sifat logika elektronik komputer yang berbasis keadaan on/off atau true/false. Dalam sistem biner, setiap posisi dari kanan mewakili pangkat 2 yang meningkat.

Contoh pada bilangan biner 1011:

- 1 paling kanan berada di posisi satuan (2⁰)
- 1 berikutnya di posisi dua (2¹)
- 0 menunjukkan tidak ada nilai di posisi empat (2²)
- 1 paling kiri di posisi delapan (2³)
