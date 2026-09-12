# 🍍 MusikNanas Notifikasi & Berita

Repository resmi untuk mengelola notifikasi push & berita di aplikasi **MusikNanas**.

## Cara Mengirim Notifikasi ke Pengguna:
Cukup edit file [`notif.json`](notif.json) langsung di GitHub (bisa lewat browser / aplikasi HP GitHub):

```json
[
  {
    "id": "2",
    "Title": "Hai disana! Ada Update Lagu Baru 🎵",
    "Description": "Daftar playlist top hits mingguan sudah diperbarui. Yuk dengarkan sekarang!",
    "ImageURL": [
      "https://raw.githubusercontent.com/nanasmuda121/MusikNanas-Notif/main/banner.png"
    ],
    "Important": true,
    "Author": "Nanas",
    "Date": 1773500000000
  }
]
```

### Penjelasan Field:
- **`id`**: Ubah ID (misal: "1", "2", "3", dst). Setiap ID baru otomatis memicu notifikasi!
- **`Title`**: Judul notifikasi yang muncul di HP (misal: `Hai disana`).
- **`Description`**: Isi pesan. Di bar notifikasi akan tampil sebagai spoiler cuplikan pesan, dan jika notifikasi ditarik ke bawah akan muncul teks lengkap.
- **`ImageURL`**: Link gambar banner (opsional, jika ada akan muncul gambar besar di notifikasi).
- **`Date`**: Timestamp milidetik (misal di-generate dari epoch time atau naikkan angkanya).
- **`Author`**: Nama pengirim (misal: `Nanas`).

Begitu kamu klik **Commit changes** di GitHub, seluruh pengguna aplikasi MusikNanas akan langsung menerima notifikasi otomatis di HP mereka! 🚀
