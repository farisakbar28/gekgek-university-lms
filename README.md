Gekgek University LMS
Gekgek University LMS adalah sebuah aplikasi Learning Management System (LMS) full-stack yang menggunakan React.js untuk front-end dan Node.js/Express.js untuk back-end, dengan PostgreSQL sebagai database. Fitur utama meliputi pengelolaan kursus, pendaftaran, komunikasi real-time menggunakan Socket.IO, otentikasi dengan JWT, dan unggahan file menggunakan Multer.

Fitur Utama
Pendaftaran Pengguna: Pengguna dapat mendaftar, masuk, dan mengelola akun mereka.

Manajemen Kursus: Admin dapat membuat, memperbarui, dan menghapus kursus.

Pendaftaran Kursus: Pengguna dapat mendaftar ke kursus yang tersedia dan mengikuti materi yang diberikan.

Manajemen Materi: Admin dapat mengunggah materi pembelajaran (video, dokumen, dll.).

Fitur Real-time: Menggunakan Socket.IO untuk chat dan interaksi real-time antara instruktur dan siswa.

Keamanan: Menggunakan JWT untuk otentikasi dan otorisasi pengguna.

File Upload: Menggunakan Multer untuk pengelolaan unggahan file dari pengguna.

Teknologi yang Digunakan
Front-End
React.js (library untuk membangun UI)

Tailwind CSS (framework untuk styling)

React Router (untuk navigasi antar halaman)

Redux (untuk manajemen state aplikasi)

Axios (untuk data fetching)

Back-End
Node.js (runtime environment)

Express.js (web framework untuk Node.js)

JWT (untuk otentikasi pengguna)

Multer (untuk manajemen file upload)

Socket.IO (untuk komunikasi real-time)

Prisma (ORM untuk interaksi dengan database PostgreSQL)

Database
PostgreSQL (relational database management system)

Testing
Jest (untuk pengujian front-end)

Mocha dan Chai (untuk pengujian back-end)

Cypress (untuk pengujian end-to-end)

Deployment
Vercel / Netlify (untuk hosting front-end)

Render / Railway (untuk hosting back-end)

Supabase (untuk hosting database)

Struktur Proyek
plaintext
.
├── client/                    # Front-end application (React)
├── server/                    # Back-end application (Node.js/Express)
├── .gitignore                 # Git ignore file
├── README.md                  # Documentation file
└── package.json               # Project dependencies and scripts
Instalasi
Untuk menjalankan aplikasi ini di lokal, ikuti langkah-langkah berikut:

Clone repositori ini:

bash
git clone https://github.com/username/repository-name.git
Install dependensi untuk client dan server: Di dalam folder client/, jalankan:

bash
npm install
Di dalam folder server/, jalankan:

bash
npm install
Konfigurasi file .env di folder server/ untuk mengatur variabel lingkungan seperti koneksi database dan JWT secret.

Jalankan server dan client: Untuk menjalankan server:

bash
npm start
Untuk menjalankan client, di folder client/, jalankan:

bash
npm run dev
Kontribusi
Kami menyambut kontribusi dari siapa saja! Jika Anda ingin berkontribusi, silakan fork repositori ini dan kirimkan pull request dengan perubahan Anda. Pastikan untuk mengikuti pedoman pengkodean dan menulis pengujian untuk fitur baru.

Lisensi
Aplikasi ini dilisensikan di bawah MIT License.
