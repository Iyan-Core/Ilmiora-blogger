# Ilmiora-blogger
Sebuah website edukasi untuk semua jaringan

Ilmiora-blog/
├── .github/
│   └── workflows/
│       └── build-cordova.yml    # (opsional) untuk build otomatis via GitHub Actions
├── www/                          # <-- folder utama untuk Cordova
│   ├── index.html                # halaman utama (kode lengkap seperti yang saya berikan)
│   ├── css/
│   │   └── style.css             (bisa dipisah)
│   ├── js/
│   │   └── app.js                (kode JavaScript API Blogger)
│   └── config.js                 (opsional, untuk API key)
├── config.xml                    # konfigurasi Cordova
├── package.json                  # dependensi dan script
├── .gitignore                    # mengabaikan platforms/, plugins/, dll
└── README.md                     # diperbarui dengan petunjuk build


# Cordova Hooks

Folder ini dapat berisi skrip yang dieksekusi pada tahap tertentu dari siklus hidup Cordova (seperti `before_build`, `after_platform_add`).  
Saat ini tidak ada hook yang digunakan. Untuk informasi lebih lanjut, lihat [Cordova Hooks Guide](https://cordova.apache.org/docs/en/latest/guide/appdev/hooks/).

## 📱 Build Aplikasi Mobile dengan Cordova

Repositori ini sudah dilengkapi file konfigurasi untuk membangun aplikasi Android/iOS menggunakan Apache Cordova. Aplikasi akan menampilkan website [Ilmiora-blog](https://lyan-core.github.io/Ilmiora-blog/) di dalam WebView, dengan akses penuh ke semua laman statis dan artikel di `ilmiora.blogspot.com`.

### Prasyarat
- Node.js dan npm terinstal
- Cordova CLI: `npm install -g cordova`
- Untuk Android: Android Studio, SDK, Java JDK 11+
- Untuk iOS: Xcode (MacOS saja)

### Langkah-langkah build

1. Clone repositori ini:
   ```bash
   git clone https://github.com/lyan-Core/Ilmiora-blog.git
   cd Ilmiora-blog
