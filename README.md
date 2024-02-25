<p align="center">
  <img height="150" height="auto" src="https://ironfish.network/img/logo.svg">
</p>

# IRONFISH HOSTING A NODE (PHASE 3)

## 1. Ikhtisar

Anda bisa mendapatkan poin dengan menghosting node penuh Iron Fish. Untuk melakukannya, pastikan telemetri Anda diaktifkan, dan grafiti Anda disetel. Anda hanya akan diberi poin untuk menghosting satu node per grafiti.

*12 jam waktu aktif terus menerus = 10 poin

Daftar: https://testnet.ironfish.network/signup

## 2. Spesifiksi Minimal

Berikut adalah persyaratan **minimum** untuk menjalankan node IRONFISH:

 -  **CPU** : 4 core
 -  **RAM** : Memori 8GB

# Instal Otomatis

```
apt update && apt upgrade -y
```

Biarkan Instalisasi Selesai, Agak Lama


```
apt install -y build-essential
```
```
apt install -y curl
```

# Cek Versi Node (Rekomendasi Versi Node v18.xx)

```
node -v
```
- Jika versi node kalian dibawah v18, Jalankan step dibawah ini, kalau sudah versi v18 lanjut ke Step ***.

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```
```
source ~/.bashrc
```
```
nvm --version
```
```
nvm ls
```
```
nvm ls-remote
```
```
nvm install v18.13.0
```

## Step ***

```
apt update && apt install yarn -y 
```
```
apt install -y nodejs 
```
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
- Pilih Y <enter>
- Pilih 1 <enter>

```
source $HOME/.cargo/env
```
(OPTIONAL)
```
npm install -global yarn --force
```
(OPTIONAL)
```
npm audit fix
```

## Clone Folder Ironfish

```
git clone https://github.com/iron-fish/ironfish
```
```
cd ironfish
```
```
yarn install
```
```
cd ironfish-cli
```
```
yarn start
```

## Pastikan Kalian Sudah Membuat Graffiti

```
yarn ironfish testnet
```
- Masukan nama Graffiti

## Membuat screen baru

```
screen -R ironfish
```

## Menjalankan Ironfish
```
yarn start start
```
- Tekan CTRL+A+D untuk keluar dari screen (berjalan di belakang background)

## Cek Status Ironfish
```
yarn ironfish status
```
- Kamu dapat mengecek Point kamu disini : https://testnet.ironfish.network/leaderboard

