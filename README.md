# NAMADA | CEREMONY
```
sudo apt update && sudo apt install -y curl git build-essential pkg-config libssl-dev
```

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
source $HOME/.cargo/env
```

Mari kita buat layarnya, karena ini adalah cara pemesanannya, agar tidak kehilangan giliran partisipasi nantinya.
 
```
screen -S ceremony
git clone https://github.com/anoma/namada-trusted-setup.git && cd namada-trusted-setup && git checkout v1.1.0
```

```
cargo build --release --bin namada-ts --features cli
```
```
mv target/release/namada-ts /usr/local/bin 
```

Sejauh ini, akan lebih mudah bagi siapa saja yang belum datang untuk menyelesaikan langkah-langkah tersebut sesudahnya. Jika Anda masih mendapat giliran, CTRL + A + Dkeluar dari layar dengan menekan tombol. Anda sekarang dapat keluar dari server secara langsung.

 

Giliran Anda ada di email Anda, jadi saat giliran Anda, ikuti langkah-langkah ini:

Mari kita ke layar dulu.

 
```
screen -r 
```

Anda mungkin mendapatkan kemungkinan kesalahan pada langkah ini: Anda melihat bahwa tidak ada layar, yaitu tidak terbuka. Anda dapat segera membuat layar baru. Kemudian Anda dapat melanjutkan ke langkah berikutnya. 

 
```
screen -S ceremony
```

Ada poin yang harus Anda perhatikan di sini. $TOKENbagian, Anda akan memasukkan token / kunci yang diberikan kepada Anda di email Anda.
Saya melempar, biarkan kunci Anda menjadi:ASDADS-ASDAE-a435345-AWEA

Perintah Anda akan terlihat seperti ini: 
```
namada-ts contribute default https://contribute.namada.net ASDADS-ASDAE-a435345-AWEA
```
 
```
namada-ts contribute default https://contribute.namada.net $TOKEN
```

Catatan: Anda akan berpartisipasi sesuai dengan tanggal di email Anda. Bergabunglah tidak terlalu dini atau terlalu terlambat. Jangan kehilangan hak :)
Bagi yang tidak bisa mendapatkan surat, [namada twitter](https://twitter.com/namadanetwork) Kami akan menunggu token dibagikan. 
Sepertinya mereka akan membagikan token harian, tetapi saya tidak tahu kapan mereka akan mulai berbagi. Anda harus cepat saat token dibagikan karena dapat dibuang dan seseorang mungkin menggunakan token yang relevan sebelum Anda melakukannya.
