# Gekgek University LMS

Gekgek University LMS adalah aplikasi Learning Management System (LMS) full-stack yang dirancang untuk mendukung proses pembelajaran daring secara efisien dan modern. Aplikasi ini memadukan teknologi terbaru untuk memberikan pengalaman pengguna yang optimal, baik bagi siswa maupun instruktur.

## Fitur Utama

- **Pendaftaran Pengguna:** Pengguna dapat mendaftar, masuk, dan mengelola akun mereka.
- **Manajemen Kursus:** Admin dapat membuat, memperbarui, dan menghapus kursus.
- **Pendaftaran Kursus:** Pengguna dapat mendaftar ke kursus yang tersedia dan mengikuti materi yang diberikan.
- **Manajemen Materi:** Admin dapat mengunggah materi pembelajaran seperti video, dokumen, dan lainnya.
- **Fitur Real-time:** Menggunakan Socket.IO untuk chat dan interaksi real-time antara instruktur dan siswa.
- **Keamanan:** Menggunakan JWT untuk otentikasi dan otorisasi pengguna.
- **File Upload:** Menggunakan Multer untuk mengelola unggahan file dari pengguna.

## Teknologi yang Digunakan

### Front-End

- React.js (library untuk membangun UI)
- Tailwind CSS (framework untuk styling)
- React Router (untuk navigasi antar halaman)
- Redux (untuk manajemen state aplikasi)
- Axios (untuk data fetching)

### Back-End

- Node.js (runtime environment)
- Express.js (web framework untuk Node.js)
- JWT (untuk otentikasi pengguna)
- Multer (untuk manajemen file upload)
- Socket.IO (untuk komunikasi real-time)
- Prisma (ORM untuk interaksi dengan database PostgreSQL)

### Database

- PostgreSQL (relational database management system)

### Testing

- Jest (untuk pengujian front-end)
- Mocha dan Chai (untuk pengujian back-end)
- Cypress (untuk pengujian end-to-end)

### Deployment

- Vercel / Netlify (untuk hosting front-end)
- Render / Railway (untuk hosting back-end)
- Supabase (untuk hosting database)

## Struktur Proyek

```
.
├── client/                    # Aplikasi Front-end (React)
│   ├── src/                   # Kode sumber aplikasi front-end
│   │   ├── redux/             # Manajemen state dengan Redux
│   │   ├── services/          # Fungsi untuk API calls (Axios)
│   │   ├── utils/             # Helper functions
│   │   ├── pages/             # Halaman utama aplikasi
│   │   ├── components/        # Komponen UI aplikasi
│   │   ├── assets/            # File aset statis (gambar, font, icon)
│   │   ├── index.jsx          # Titik masuk utama aplikasi React
│   │   ├── App.jsx            # Komponen utama aplikasi
│   │   ├── index.css          # CSS global
│   ├── public/                # File statis, termasuk index.html
│   ├── .gitignore             # File Git ignore khusus client
│   ├── tailwind.config.js     # Konfigurasi Tailwind CSS
│   ├── postcss.config.js      # Konfigurasi PostCSS
│   ├── package.json           # Dependensi dan skrip front-end
│   ├── package-lock.json      # Versi pasti dependensi front-end
│   ├── README.md              # Dokumentasi client-side
│   ├── vite.config.js         # Konfigurasi Vite bundler
│   └── eslint.config.js       # Konfigurasi ESLint
├── server/                    # Aplikasi Back-end (Node.js/Express)
│   ├── prisma/                # Skema Prisma ORM untuk database
│   │   └── schema.prisma      # Definisi skema database
│   ├── config/                # File konfigurasi aplikasi
│   ├── utils/                 # Fungsi utilitas di sisi server
│   ├── middleware/            # Middleware seperti autentikasi
│   ├── services/              # Logika utama aplikasi (user, course, file)
│   ├── routes/                # Rute API
│   ├── models/                # Model Prisma untuk database
│   ├── controllers/           # Logika untuk menangani request dan response
│   ├── server.js              # Titik masuk utama untuk server back-end
│   ├── .gitignore             # File Git ignore khusus server
│   ├── .env                   # Variabel lingkungan (mis. database, JWT secret)
│   ├── package.json           # Dependensi dan skrip back-end
│   └── package-lock.json      # Versi pasti dependensi back-end
├── .gitignore                 # Git ignore untuk root folder
├── package.json               # Dependensi dan skrip proyek utama
└── package-lock.json          # Versi pasti dependensi proyek utama
```

## Cara Instalasi

### 1. Clone Repository

Clone repository ini ke komputer Anda:

```bash
git clone https://github.com/farisakbar28/gekgek-university-lms.git
```

### 2. Instal Dependensi

- Masuk ke folder `client/` dan jalankan:
  ```bash
  npm install
  ```
- Masuk ke folder `server/` dan jalankan:
  ```bash
  npm install
  ```

### 3. Konfigurasi File .env

Buat file `.env` di folder `server/` dengan isi berikut:

```
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
```

### 4. Jalankan Aplikasi

- Untuk menjalankan server:
  ```bash
  npm start
  ```
- Untuk menjalankan client (di folder `client/`):
  ```bash
  npm run dev
  ```
- Untuk menjalankan client dan server secara bersamaan:
  ```bash
  npm run dev
  ```

## Kontribusi

Kami menyambut kontribusi dari siapa saja! Jika Anda ingin berkontribusi, silakan fork repository ini dan kirimkan pull request dengan perubahan Anda. Pastikan untuk mengikuti pedoman pengkodean dan menulis pengujian untuk fitur baru.

## Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).
