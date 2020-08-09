# Instalasi React Native pada Sistem Operasi Mac

1. Install `Homebrew`

```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

$ brew --version
```

2. Install `NodeJs`dan `Watchman`

```
$ brew install node
$ brew install watchman
$ node --version
$ watchman --version
```

3. Install `Java Development Kit`

```
$ brew cask install adoptopenjdk/openjdk/adoptopenjdk8
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

7. Menambahkan direktori `~/Library/Android/Sdk` ke dalam file `~/.bash_profile` , agar perintah android dapat digunakan pada terminal.

- Buka file `~/.bash_profile` dengan nano

```
$ nano ~/.bash_profile
```

- Lalu pada bagian akhir tambahkan baris ini

```
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

- Tekan `Ctrl+x` untuk keluar dan pilih `y` untuk menyimpan

8. Muat konfigurasi pada terminal

```
$ source .bash_profile
```

9. Cek Lokasi `Android`

```
$ echo $ANDROID_HOME
```

10. Buat Proyek Aplikasi

```
$ npx react-native init NamaAplikasi
```
