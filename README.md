# UwUrg

Port dari [turg](https://github.com/commrade-goad/turg) dari C ke C++ untuk proyek `OOP Class`.

[Link Repositori](https://github.com/commrade-goad/uwurg)

## Library yang Digunakan

- [raylib](https://github.com/raysan5/raylib)

## Cara Build

### Windows

Anda dapat mengunduh rilisan aplikasi pada bagian `tags`.  
Saat ini aplikasi belum dalam versi final, namun Anda dapat mencoba versi `pre-release`.  
Unduh file bernama `rc1-x86_64-win32.zip`, ekstrak ke folder pilihan Anda,  
kemudian buka folder `UwUrg's Release` dan jalankan `uwurg.exe`.

### Arch Linux

Install dependensi:

```sh
sudo pacman -S base-devel clang glu cmake libx11 git libglvnd gcc-libs libxcb libxau libxdmcp libxcursor libxinerama libxrandr
```

### Ubuntu / Linux Mint

#### Install dari Release

Anda dapat mengunduh rilisan aplikasi pada bagian `tags`.  
Saat ini aplikasi belum dalam versi final, namun Anda dapat mencoba versi `pre-release`.  
Unduh file bernama `rc1-x86_64-linux.zip`, ekstrak ke folder pilihan Anda,  
lalu buka folder `UwUrg's Release` dan jalankan `uwurg`.

#### Build dari Source

Install dependensi:

```bash
sudo apt install -y cmake libgl1-mesa-dev libglu1-mesa-dev libx11-dev libxcb1-dev libxau-dev libxdmcp-dev libxrandr-dev libxinerama-dev libxcursor-dev libxi-dev libasound2-dev git build-essential clang
```

> **Catatan:**  
> Disarankan untuk menginstal `cmake` melalui **Snap** agar mendapatkan versi terbaru (versi dari apt biasanya sudah usang):

```bash
sudo snap install cmake --classic
```

### Build (Berlaku untuk Semua Sistem)

```sh
git clone https://github.com/commrade-goad/uwurg
cd uwurg
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release .. # atau gunakan `Debug` untuk build debug
make -j$(nproc)
cd ..
./build/uwurg
```
