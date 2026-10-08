# Laporan Praktik Git Merge Conflict - LKPD 6

**Anggota Tim:**
- Sabrina
- Fajrillah

---

## C. Misi 1: Memahami Merge Conflict
Merge Conflict adalah kondisi ketika Git tidak dapat menggabungkan dua branch secara otomatis karena terdapat perubahan yang saling bertabrakan pada file dan baris kode yang sama di branch berbeda.

---

## F. Misi 4: Membaca Penanda Conflict
- `<<<<<<< HEAD`: Menandakan awal kode dari branch yang sedang aktif saat ini (`main`).
- `=======`: Garis pembatas antara kode di branch saat ini dengan kode dari branch yang digabungkan.
- `>>>>>>> fitur-header-b`: Akhir dari kode yang berasal dari branch `fitur-header-b`.

---

## H. Checkpoint 1 (Evaluasi Praktik)
- [v] Skenario branch `fitur-header-a` dan `fitur-header-b` berhasil dibuat.
- [v] Anggota tim berhasil melihat pesan peringatan Merge Conflict di terminal.
- [v] File berhasil disatukan kembali dan di-commit tanpa meninggalkan sisa karakter penanda.
- [v] Log graph menunjukkan cabang yang berpisah dan menyatu kembali (3-way merge).
 
 [v] Screenshot Terminal saat terjadi pesan CONFLICT

[v] Screenshot Text Editor (VS Code) yang menampilkan penanda <<<<<<< HEAD

[v] Screenshot hasil analisis git log --graph --oneline --all yang menunjukkan merge
---

## I. Simulasi Masalah (Studi Kasus)

### Kasus 1
Perintah Git yang digunakan Budi untuk membatalkan proses merge dan kembali ke posisi aman:
```bash
git merge --abort

###kasus 2
Tidak. karena merge conflict itu bukan berarti  masing masing anggota tim melakukan kesalahan. Conflict adalah hal yang wajar dalam kolaborasi tim saat dua orang mengedit baris kode yang sama. Git sengaja menghentikan proses penggabungan agar tim berdiskusi untuk menentukan kode mana yang ingin dipertahankan.