# Hallo teman teman saya
Nama : Muhamad David Ali

NIM : 312210291

Kelas : TI.22.A1
## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Tugas ke-9|[Click Here](https://github.com/Luxcario/praktikum6/edit/main/README.md#tugas-ke-9)|
|2|Flowchart tugas ke-9|[Click Here](https://github.com/Luxcario/praktikum6/edit/main/README.md#flowchart-tugas-ke-9)|


## Tugas ke-6
Buatlah program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut :

- Fungsi tambah() untuk menambahkan data
- Fungsi tampilan() untuk menampilkan data  
- Fungsi hapus() untuk menghapus data berdasarkan nama
- Fungsi ubah() untuk mengubah data bersadarkan nama
- Buat flowchart dan penjelasan programnya pada README.md.
- Commit dan push repository ke github.

#### Langkah-langkah :
1. Buatlah programnya terlebih dahulu seperti gambar di bawah ini

```
from os import system
s_nama = []
s_nim = []
s_tugas = []
s_uts = []
s_uas = []
s_akhir = []


def judul():
    print('==================================')
    print('|     Daftar Nilai Mahasiswa     |')
    print('==================================')


def menu():
    system('cls')
    print('=====================================')
    print('Input Data Nilai Mahasiswa'.center(40))
    print('=====================================')
    print('|    1. Tambah Data                 |')
    print('|    2. Tampilkan Data Mahasiswa    |')
    print('|    3. Ubah Data Mahasiswa         |')
    print('|    4. Hapus Data Mahasiswa        |')
    print('|    5. Selesai                     |')
    print('=====================================')
    choose = input('Pilih Menu  : ')
    if choose == '1':
        tambah()
    elif choose == '2':
        tampilkan()
    elif choose == '3':
        ubah()
    elif choose == '4':
        hapus()
    elif choose == '5':
        selesai()
    else:
        tidak = input('Menu Tidak Ada')
        system('cls')
        menu()


def tambah():
    system('cls')
    judul()
    print('Tambah Data'.center(40))
    print('==================================')
    nama = input('Nama     : ')
    s_nama.append(nama)
    nim = input('NIM       : ')
    s_nim.append(nim)

    system('cls')
    judul()
    print('Tambah Data'.center(40))
    print('==================================')
    tugas = float(input('Nilai Tugas    : '))
    s_tugas.append(tugas)

    uts = float(input('Nilai UTS        : '))
    s_uts.append(uts)

    uas = float(input('Nilai UAS        : '))
    s_uas.append(uas)

    total = tugas * 0.30 + uts * 0.35 + uas * 0.35
    s_akhir.append(total)
    print('Data Tersimpan'.center(40))
    kembali = input('Kembali [Enter]')
    menu()


def tampilkan():
    system('cls')
    judul()

    for i in range(len(s_nim)):
        print('%d. Nama         : %s' % (i + 0, s_nama[i]))
        print('    NIM          : %s' % s_nim[i])
        print('    Nilai Tugas  : %.2f' % s_tugas[i])
        print('    UTS          : %.2f' % s_uts[i])
        print('    UAS          : %.2f' % s_uas[i])
        print('    Nilai Akhir  : %.2f' % s_akhir[i])
        print('-----------------------------')
    kembali = input('Kembali Tekan [Enter]')
    menu()


def ubah():
    rubah = input('Ubah Biodata Tekan [B]   : ')
    if rubah == 'B' or rubah == 'b':
        i = int(input('Masukkan Nomor Urut  : '))
        if (i > len(s_nim[i])):
            print('Nomor Urut Salah')
        else:
            namabaru = input('Nama      : ')
            s_nama[i] = namabaru
    kembali = input('Kembali Tekan [Enter]')
    menu()


def hapus():
    system('cls')
    judul()
    print('Hapus Data'.center(40))
    print('=================================')
    i = int(input('Masukkan Nomor Urut  : '))

    if (i > len(s_nim[i])):
        tidak = input('NIM Tidak Ada')
        hapus()

    else:
        s_nim.remove(s_nim[i])
        s_nama.remove(s_nama[i])
        s_tugas.remove(s_tugas[i])
        s_uts.remove(s_uts[i])
        s_uas.remove(s_uas[i])
        s_akhir.remove(s_akhir[i])

    print('Data Berhasil Di Hapus')
    kembali = input('Kembali Tekan [Enter]')
    menu()


def selesai():
    system('cls')
    menu()
```

menu()

![image](https://user-images.githubusercontent.com/116184002/206187743-a530f87d-2433-4d6f-8c4c-1c3fc0e51885.png)
![image](https://user-images.githubusercontent.com/116184002/206187803-b5485ba5-14aa-47f3-a975-8494f1414f66.png)
![image](https://user-images.githubusercontent.com/116184002/206187838-919afb15-40c9-4b10-bd2f-ca61081ab9ac.png)
![image](https://user-images.githubusercontent.com/116184002/206187886-1a5fc6dd-6e75-42ff-b5d2-68e7d752c138.png)
![image](https://user-images.githubusercontent.com/116184002/206187984-b97e6e01-9f38-4a6f-94bb-97132a5f4881.png)
![image](https://user-images.githubusercontent.com/116184002/206187997-2b9e9999-29a3-4b32-a85a-d1f3daf93aac.png)

    
    
2. langkah-langkah

 1.menambahkan data
 ![image](https://user-images.githubusercontent.com/116184002/206189515-4c078360-fa66-4283-b870-e8901100fdff.png)


 
 2.menampilkan data
 ![image](https://user-images.githubusercontent.com/116184002/206189629-c6afc7f9-0b1d-4d32-b932-f676f1363e34.png)

 
 3.menghapus data
 ![image](https://user-images.githubusercontent.com/116184002/206190099-cdfe74e4-cf3b-4979-b976-330183b68b9b.png)
 ![image](https://user-images.githubusercontent.com/116184002/206190084-9111794b-6dad-40e7-bd84-05f63b2ee562.png)
 
 4.mengubah data
 ![image](https://user-images.githubusercontent.com/116184002/206190698-39704fbf-adfe-4b12-ad0e-337d294376f7.png)
 ![image](https://user-images.githubusercontent.com/116184002/206190720-37ea19f1-74a5-497a-b0a0-b6611d6d0f9b.png) 










### Penjelasan Program :
1. pilih 1 untuk menambahkan data masukkan nama , nim, nilai tugas, nilai UTS, nilai uUAS lalu enter(tambahkan 1 biodata lagi bebas)
2. pilih menu 2 untuk menampilkan data
3. pilih menu 4 untuk menghapus data, lalu pilih no urut yang akan di hapus
4. pilih 3 untuk mengubah, lalu takn B, lalu ganti nama 
5. Selesai

### Flowchart tugas ke-9
![image](https://user-images.githubusercontent.com/116184002/206192719-78d31773-642b-4974-b58d-36f42e5d3d55.png)




### Sekian Terimakasih 
