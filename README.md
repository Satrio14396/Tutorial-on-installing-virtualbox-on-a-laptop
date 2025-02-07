# Tutorial-on-installing-virtualbox-on-a-laptop
# Tutorial Instalasi VirtualBox di Laptop

Tutorial ini akan memandu kamu melalui langkah-langkah untuk menginstal VirtualBox di laptop. Ikuti langkah-langkah dengan hati-hati dan lihat tangkapan layar untuk pemahaman yang lebih baik.

## Persyaratan Sistem
Sebelum menginstal VirtualBox, pastikan laptop yang kamu pakai memenuhi persyaratan berikut:
- Prosesor 64-bit dengan dukungan virtualisasi (Intel VT-x atau AMD-V diaktifkan di BIOS)
- Minimal RAM 4GB (disarankan 8GB untuk performa lebih baik)
- Minimal 10GB ruang kosong di hard disk
- Sistem operasi Windows, macOS, atau Linux

## Panduan Instalasi Langkah demi Langkah

### Langkah 1: Unduh VirtualBox
1. Buka browser web di laptop dan kunjungi [situs resmi VirtualBox](https://www.virtualbox.org/).
2. Klik **Download VirtualBox**.
![Screenshot 2025-02-07 202833](https://github.com/user-attachments/assets/a6426192-357d-4e97-a669-9d6a9c0e9620)
3.Pilih versi sesuai dengan sistem operasi yang kamu gunakan (Windows, macOS, atau Linux).
![Screenshot 2025-02-07 202851](https://github.com/user-attachments/assets/7beccfca-fd5c-4eab-9ab6-d47024743f2e)

### Langkah 2: Instal VirtualBox
#### Untuk Windows:
1. Cari file `.exe` yang telah diunduh dan klik dua kali untuk menjalankannya.
  ![Screenshot 2025-02-07 203711](https://github.com/user-attachments/assets/6c411dff-a860-4896-bd2f-af27da1dfecd)

3. Ikuti panduan instalasi dan klik **Next** untuk melanjutkan.
4. Biarkan pengaturan default kecuali kamu memerlukan konfigurasi khusus.
5. Klik **Install** dan tunggu hingga proses selesai.
6. Klik **Finish** untuk menutup installer.

#### Untuk macOS:
1. Buka file `.dmg` yang telah diunduh.
2. Seret ikon VirtualBox ke dalam folder **Applications**.
3. Buka VirtualBox dari folder Applications.
4. Jika muncul peringatan, izinkan akses di **System Preferences > Security & Privacy**.

#### Untuk Linux (Ubuntu/Debian-based):
1. Buka terminal dan jalankan perintah berikut:
   ```bash
   sudo apt update
   sudo apt install virtualbox -y
   ```
2. Tunggu hingga instalasi selesai.
3. Verifikasi instalasi dengan menjalankan:
   ```bash
   virtualbox
   ```

### Langkah 3: Instal VirtualBox Extension Pack (Opsional)
1. Kembali ke [situs VirtualBox](https://www.virtualbox.org/).
2. Unduh Extension Pack yang sesuai dengan versi VirtualBox Anda.
3. Buka VirtualBox dan masuk ke **File > Preferences > Extensions**.
4. Klik **Add New Package** dan pilih Extension Pack yang telah diunduh.
5. Klik **Install** dan setujui perjanjian lisensi.

Nah sebelum kita membuat virtual machine nya kita di haruskan sudah mendownload file ISO sistem operasi, sebagai contoh:ubuntu
![Screenshot 2025-02-07 212019](https://github.com/user-attachments/assets/aeec1ae8-d131-49d6-acf2-923c71e6ea89)
![Screenshot 2025-02-07 211942](https://github.com/user-attachments/assets/501a1a65-b18d-44c3-b012-4ae9ea061c7e)
![Screenshot 2025-02-07 211957](https://github.com/user-attachments/assets/cfe759fd-1349-4d2d-9205-b0a76d6aa7cd)

# Tutorial Setting Virtual Machine di VirtualBox

Tutorial ini akan memandu kamu dalam mengatur Virtual Machine (VM) di VirtualBox setelah instalasi.

## **Langkah 1: Membuka VirtualBox dan Membuat Virtual Machine Baru**
1. Buka **VirtualBox**.
2. Klik tombol **New** untuk membuat VM baru.
3. Masukkan **nama** VM (contoh: "Ubuntu-Linux"), lalu pilih:
   - **Type**: Sistem operasi yang ingin diinstal (Windows, Linux, macOS, dll.)
   - **Version**: Pilih versi OS yang sesuai (contoh: Ubuntu 64-bit).
4. Klik **Next**.
   ![Screenshot 2025-02-07 212701](https://github.com/user-attachments/assets/fcb14363-d1bf-4f01-8b3b-ab1cc1976f46)
![Screenshot 2025-02-07 213401](https://github.com/user-attachments/assets/1e112806-f497-4920-8ff2-5fb4f31088b9)


## **Langkah 2: Mengatur Alokasi RAM**
1. Tentukan jumlah RAM yang ingin dialokasikan ke VM.
   - **Minimal 2GB (2048MB) untuk Linux ringan**.
   - **Disarankan 4GB atau lebih untuk Windows dan Linux berat**.
2. Klik **Next**.
![Screenshot 2025-02-07 212820](https://github.com/user-attachments/assets/3e5feafd-2c03-4c35-8513-544bf014bd0d)

## **Langkah 3: Membuat Hard Disk Virtual**
1. Pilih **Create a virtual hard disk now** lalu klik **Create**.
2. Pilih format disk virtual:
   - **VDI (VirtualBox Disk Image)** – Default, cocok untuk kebanyakan pengguna.
   - **VHD atau VMDK** jika ingin kompatibel dengan software lain.
3. Pilih metode alokasi ruang:
   - **Dynamically allocated** (lebih fleksibel, hanya menggunakan ruang saat diperlukan).
   - **Fixed size** (lebih cepat, tapi langsung mengambil semua ruang yang dialokasikan).
4. Tentukan ukuran disk (disarankan minimal **20GB** untuk Linux dan **50GB** untuk Windows).
5. Klik **Create**.

## **Langkah 4: Mengatur Konfigurasi Tambahan (Opsional)**
Sebelum menjalankan VM, bisa dilakukan pengaturan tambahan:
1. Pilih VM yang sudah dibuat, lalu klik **Settings**.![Screenshot 2025-02-07 213436](https://github.com/user-attachments/assets/53422668-dc95-46e1-a74f-c9ee647d0296)

2. Pada tab **System**, aktifkan **Enable EFI (special OSes only)** jika diperlukan.
3. Pada tab **Display**, atur **Video Memory** menjadi 128MB untuk performa grafis yang lebih baik.
4. Pada tab **Storage**, tambahkan **file ISO sistem operasi** yang ingin diinstal.![Screenshot 2025-02-07 213811](https://github.com/user-attachments/assets/bbaa0358-be2a-4349-b2a9-e86e4bad5a11)
![Screenshot 2025-02-07 213840](https://github.com/user-attachments/assets/2d2e4251-8352-4fa4-8b12-e19d67df31e5)

5. Klik **OK** untuk menyimpan pengaturan.

## **Langkah 5: Menjalankan Virtual Machine**
1. Pilih VM yang sudah dikonfigurasi.
2. Klik **Start** untuk menjalankan mesin virtual.![Screenshot 2025-02-07 213943](https://github.com/user-attachments/assets/fc1a7cd2-6918-4876-9a02-277de7c33145)

3. Ikuti instruksi instalasi sistem operasi sesuai dengan OS yang dipilih.![bllll](https://github.com/user-attachments/assets/f8f26896-496b-4350-8522-bc34dd79747f)


## **Kesimpulan**
Kamu telah berhasil mengatur Virtual Machine di VirtualBox. Semoga langkah langkah nya membantu..


