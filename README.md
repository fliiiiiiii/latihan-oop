# Nama    : Rafli Anugrah Ramadhan
# Kelas   : TI.24.A4
# NIM     : 312410351
# Matkul  : Bahasa Pemrograman

# Latihan 1

![image](https://github.com/user-attachments/assets/d67e470c-e989-45e9-96d1-59c5d3dd742d)

# Kode program

# Data/mahasiswa.py

<img width="497" alt="image" src="https://github.com/user-attachments/assets/5910cc77-3b43-456e-b5a3-9a7a31e6bfa9">

<img width="438" alt="image" src="https://github.com/user-attachments/assets/a6f66448-e5d6-4514-8e7f-43b0e6e8f81e">

Class DaftarNilaiMahasiswa:

__init__: Menyimpan data mahasiswa dalam bentuk dictionary.

tambah_data(): Menambahkan data baru berdasarkan input pengguna.

tampilkan_data(): Menampilkan semua data mahasiswa dalam format tabel sederhana.

hapus_data(): Menghapus data mahasiswa berdasarkan nama.

ubah_data(): Mengubah nilai tugas, UTS, dan UAS mahasiswa.

# view/input.from

<img width="321" alt="image" src="https://github.com/user-attachments/assets/b57c8bf4-babc-4bcf-805d-c687984fac69">

# view/mahasiswa.py

<img width="398" alt="image" src="https://github.com/user-attachments/assets/a79f17f2-d7ce-4183-ac4c-883786c68e98">

# main.py

<img width="500" alt="image" src="https://github.com/user-attachments/assets/963276ec-491e-4c49-8d4a-f8bc197a9eb5">

# penjelasan
    Package data: Menangani data dan logika manajemen mahasiswa.
    Package view: Menangani interaksi dengan pengguna (input/output).
    File main.py: Menjalankan aplikasi dan mengintegrasikan modul yang dibuat.

Dalam Python, file __init__.py adalah file khusus yang digunakan untuk menunjukkan bahwa direktori tertentu adalah sebuah package. Ada beberapa alasan mengapa file __init__.py sering dibiarkan kosong, terutama dalam konteks seperti contoh di atas:
1. Tidak Ada Logika yang Dibutuhkan di __init__.py

    Dalam struktur proyek tersebut, file __init__.py tidak memerlukan logika tambahan karena semua kode dan fungsionalitas sudah didefinisikan di modul lain (misalnya
```python
mahasiswa.py, input_form.py).
    Tujuannya hanyalah untuk menunjukkan bahwa direktori data dan view adalah package Python yang valid.
````
3. Menggunakan __init__.py Sebagai Indikator Package

    Secara teknis, sejak Python 3.3, file __init__.py tidak lagi diwajibkan untuk mendeklarasikan package. Namun, tetap disarankan untuk menyertakan file ini, meskipun kosong, agar kompatibel dengan versi Python yang lebih lama atau untuk menambah kejelasan struktur proyek.

4. Kapan __init__.py Tidak Kosong?

Ada beberapa skenario di mana Anda mungkin menambahkan kode ke dalam __init__.py:

    Ekspor Simbol: Untuk menentukan apa yang akan diimpor saat menggunakan from package import *.

from .mahasiswa import Mahasiswa, DataMahasiswa

Logika Inisialisasi Package: Jika package membutuhkan konfigurasi awal.
Shortcut Import: Untuk mempermudah impor modul dengan menyediakannya langsung di level package. Misalnya:
```python
    # __init__.py di folder view
    from .input_form import InputForm
    from .mahasiswa import ViewMahasiswa
````

# Hasil Program

<img width="171" alt="image" src="https://github.com/user-attachments/assets/e635cfe9-9971-4e99-ba57-4e5cac3f8e98">

![image](https://github.com/user-attachments/assets/f813cb1a-1f3c-4ad9-87a6-347a4f582276)

![image](https://github.com/user-attachments/assets/df2594bc-34d4-463b-88f6-5a10be13c614)

































