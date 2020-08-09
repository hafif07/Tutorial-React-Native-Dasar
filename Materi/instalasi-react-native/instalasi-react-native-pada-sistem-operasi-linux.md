# Instalasi React Native pada Sistem Operasi Linux

1. Install `NodeJs`

```
$ sudo apt update
$ sudo apt install nodejs
$ nodejs -v
```

2. Install `npm`

```
$ sudo apt install npm
$ npm -v
```

3. Install `Java Development Kit`

```
$ sudo apt install openjdk-8-jdk openjdk-8-jdk-headless openjdk-8-jre
```

4. Cek `JDK`

```
$ javac -version
```

5. Cek `JRE`

```
$ java -version
```

6. Install `Android SDK`

7. Menambahkan direktori `~/Android/Sdk` ke dalam file `~/.bashrc` , agar perintah android dapat digunakan pada terminal.

- Buka file `~/.bashrc` dengan nano

```
$ nano ~/.bashrc
```

- Lalu pada bagian akhir tambahkan baris ini

```
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

- Tekan `Ctrl+x` untuk keluar dan pilih `y` untuk menyimpan

8. Muat konfigurasi pada terminal

```
$ source .bashrc
```

9. Cek Lokasi `Android`

```
$ echo $ANDROID_HOME
```

10. Buat Proyek Aplikasi

```
$ npx react-native init NamaAplikasi
```
