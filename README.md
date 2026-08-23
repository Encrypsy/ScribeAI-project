# ScribeAI

**ScribeAI** adalah aplikasi web berbasis Django yang mengubah video YouTube menjadi artikel blog secara otomatis menggunakan kecerdasan buatan. Cukup masukkan link video YouTube, dan ScribeAI akan mentranskripsikan audionya lalu menyusunnya menjadi artikel blog yang rapi dan siap dibaca.

## Fitur

-  **Autentikasi pengguna** — sistem login dan register
-  **Input link YouTube** — cukup tempel link video, tidak perlu upload manual
-  **Transkripsi otomatis** — audio video diubah menjadi teks menggunakan [AssemblyAI](https://www.assemblyai.com/)
-  **Generate artikel dengan AI** — teks transkrip diolah menjadi artikel blog yang terstruktur dan enak dibaca
-  **Indikator loading** — status proses ditampilkan secara real-time selama artikel sedang dibuat
-  **Antarmuka responsif** — dibangun dengan Tailwind CSS, mendukung tampilan mobile maupun desktop

##  Tech Stack

| Kategori | Teknologi |
|---|---|
| Backend | Django (Python) |
| Frontend | HTML, Tailwind CSS, JavaScript |
| Speech-to-Text | AssemblyAI API |
| AI Content Generation | LLM API |
| Database | *(sesuaikan, misal: SQLite / PostgreSQL)* |

##  Instalasi

```bash
# Clone repository
git clone https://github.com/Encrypsy/scribeai.git
cd scribeai

# Buat virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Buat file .env dan isi API key yang dibutuhkan
# ASSEMBLYAI_API_KEY=your_api_key_here

# Jalankan migrasi database
python manage.py migrate

# Jalankan server
python manage.py runserver
```

Aplikasi akan berjalan di `http://127.0.0.1:8000/`

## ⚙️ Environment Variables

Buat file `.env` di root project dan tambahkan:

```
ASSEMBLYAI_API_KEY=your_assemblyai_api_key
SECRET_KEY=your_django_secret_key
```

##  Author

**Malya Maritza**
GitHub: [@Encrypsy](https://github.com/Encrypsy)
