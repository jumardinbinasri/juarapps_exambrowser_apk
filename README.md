# APK ExamBrowser (publik)

Repo ini HANYA menyimpan file APK terbaru agar HP bisa download.
Kode sumber tetap di repo privat.

## Cara rilis versi baru (cukup web GitHub, tanpa perintah)

1. Buka **Releases** -> **Create a new release**.
2. Tag: `v1.2.0+2081` (samakan angka dengan versi di aplikasi).
3. Seret 1 file `.apk` (nama harus mengandung versi, cth.
   `ExamBrowser-v1.2.0+2081.apk`) -> **Publish release**.
4. Selesai. Halaman admin -> tab Update Aplikasi ->
   **Ambil dari GitHub** -> **Simpan**.

## Otomatis isi database (opsional, sekali saja)

Tambahkan 2 secret di repo ini (Settings -> Secrets -> Actions):
`SUPABASE_URL` dan `SUPABASE_SERVICE_ROLE_KEY` (lihat repo privat).
Setelah itu tiap Release terbit, database terisi sendiri.

## File app-update.json

Catatan versi terbaru (cadangan bila API Release tidak terbaca).
Diperbarui otomatis oleh workflow, atau edit manual di web.