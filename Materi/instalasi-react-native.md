# Instalasi React Native

`Perhatian !!!` Tutorial instalasi yang saya buat menggunakan sistem operasi `Linux` , jika kamu menggunakan sistem operasi lain `windows or mac` kamu bisa cari referensinya di bawah ini :
 - [Windows](https://www.dumetschool.com/blog/Cara-Menginstal-React-Native-Android-Pada-Windows)
 - [Mac](https://medium.com/@bangkit/instal-react-native-di-mac-os-63a5edcb9d49)


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
3. Install `Java JDK `
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
8. Cek `Android Version`
```
$ android --version
```
9. Install `React Native`
```
$ sudo npm install -g react-native-cli
```