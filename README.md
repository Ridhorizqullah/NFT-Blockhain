### ✅ `README.md` 

```markdown
# Praktikum NFT – Smart Contract ERC-721

Proyek ini merupakan implementasi smart contract **Non-Fungible Token (NFT)** berbasis standar **ERC-721** menggunakan **Solidity** dan **OpenZeppelin**, dikembangkan dalam lingkungan **Truffle** dan diuji pada **Ganache**.

## 📁 Struktur Direktori

```
nft-praktikum/
├── contracts/
│   └── MyNFT.sol             # Smart contract NFT
├── migrations/
│   └── 1_deploy_contracts.js # Script deploy
├── truffle-config.js         # Konfigurasi jaringan
└── package.json
```

## ⚙️ Prasyarat

- Node.js (disarankan v18.x)
- Truffle: `npm install -g truffle`
- Ganache (CLI atau GUI)
- Ekstensi MetaMask (opsional, untuk integrasi)

## ▶️ Cara Menjalankan

1. Masuk ke direktori proyek:
   ```bash
   cd nft-praktikum
   ```

2. Instal dependensi:
   ```bash
   npm install
   ```

3. Jalankan Ganache secara lokal (pastikan berjalan di port `7545`).

4. Deploy smart contract ke jaringan lokal:
   ```bash
   truffle migrate --network development
   ```

5. (Opsional) Uji interaksi dengan contract via Truffle console:
   ```bash
   truffle console --network development
   ```

## 📜 Fitur Smart Contract

- Mewarisi `ERC721` dan `ERC721URIStorage` dari OpenZeppelin
- Menggunakan `Counters` untuk autogenerasi token ID
- Hanya owner yang bisa melakukan `mint`
- Mendukung penyimpanan metadata NFT melalui URI (misal: IPFS, JSON)

## 🌐 Deploy ke Testnet (Sepolia)

Untuk deploy ke jaringan Sepolia:

1. Tambahkan file `.env`:
   ```env
   MNEMONIC="kalimat seed wallet Anda"
   INFURA_PROJECT_ID="id_proyek_infura"
   ```

2. Pastikan `truffle-config.js` sudah dikonfigurasi untuk jaringan `sepolia`.

3. Jalankan:
   ```bash
   truffle migrate --network sepolia
   ```

## 📚 Referensi

- [OpenZeppelin ERC721](https://docs.openzeppelin.com/contracts/4.x/erc721)
- [Truffle Suite Docs](https://trufflesuite.com/docs/)
- [Ethereum ERC-721 Standard](https://eips.ethereum.org/EIPS/eip-721)

---

© 2025 – Praktikum Blockchain, Program Studi Teknologi Informasi  
Universitas Muhammadiyah Yogyakarta
```

---

Jika kamu bisa memberikan **daftar file** atau **isi `contracts/`**, saya bisa buatkan README yang **lebih akurat dan spesifik**. Atau, jika ini bagian dari **tugas kelompok/praktikum**, sesuaikan nama file dan deskripsi sesuai dengan implementasimu!
