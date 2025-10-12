# Priority Queue and Heap

## What is the relationship between priority queue and heap?

Priority Queue is an Abstract Data Type, and Heap is the concrete data structure we use to implement a priority queue

## Priority Queue

Priority queue adalah struktur data yang terdiri dari sekumpulan item dan mendukung operasi berikut:

- insert: memasukkan item dengan sebuah key.
- delete_min/delete_max: menghapus item dengan key terkecil/terbesar dan mengembalikannya.

Perlu dicatat bahwa

kita hanya dapat mengambil dan menghapus elemen dengan key min/max dan TIDAK sembarang key.

## Use cases

Proses triase di rumah sakit adalah contoh utama penggunaan priority queue. Pasien diurutkan berdasarkan tingkat keparahan kondisinya. Misalnya, seseorang dengan flu datang dan ditempatkan di akhir antrian. Kemudian, seseorang yang mengalami kecelakaan mobil datang dan ditempatkan sebelum orang dengan flu meskipun datang belakangan karena kondisinya lebih parah. Dalam kasus ini, tingkat keparahan menjadi key.

Pertimbangkan masalah seperti Merge K sorted lists. Kita perlu melacak nilai minimum di antara k elemen (elemen terkecil dari setiap list yang sudah terurut) dan menghapus nilai minimum serta memasukkan nilai baru kapan saja, sambil tetap dapat mengakses nilai minimum setiap saat. Berikut beberapa masalah lain di mana priority queue sangat berguna:

- k closest points to origin <https://leetcode.com/problems/k-closest-points-to-origin/>
- kth largest element <https://leetcode.com/problems/kth-largest-element-in-an-array/>
- kth largest element in a stream <https://leetcode.com/problems/kth-largest-element-in-a-stream/>
- Median of a data stream <https://leetcode.com/problems/find-median-from-data-stream/>
- Uniform Cost Search <https://algo.monster/problems/uniform-cost-search>

## Implement Priority Queue using an array

Untuk melakukan ini, kita bisa mencoba menggunakan:

- Array tak terurut (unsorted array): operasi insert akan memiliki kompleksitas waktu O(1) karena kita cukup menambahkan elemen di akhir array. Namun, untuk menemukan dan menghapus nilai minimum, kompleksitasnya menjadi O(N) karena kita harus melakukan iterasi ke seluruh elemen array untuk menemukannya.
- Array terurut (sorted array): menemukan nilai minimum menjadi mudah dengan kompleksitas O(1), tetapi operasi insert akan memakan waktu O(N) karena kita harus mencari posisi yang tepat untuk nilai tersebut, lalu menggeser elemen-elemen setelahnya untuk memberi ruang dan menyisipkan nilai ke posisi tersebut.
