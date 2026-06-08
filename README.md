# 🟥 IM Training — Template Kerja Tim

Repo ini digunakan oleh tim Information Management (IM) untuk mengelola tasking, progres kerja, output, dan dokumentasi keputusan selama latihan atau operasi respons bencana.

Repo ini dapat dipakai bersama **Microsoft Teams**, **SharePoint**, dan **GitHub Project Kanban**. Teams digunakan untuk komunikasi dan koordinasi. SharePoint digunakan untuk penyimpanan dokumen kerja. GitHub digunakan untuk tasking, pelacakan progres, dan dokumentasi kerja.

---

## 📈 Progress Project Kanban

<!-- PROJECT_PROGRESS:START -->
![Progress](https://geps.dev/progress/0)

**Progress Kanban:** 0/0 item selesai (0%).
<!-- PROJECT_PROGRESS:END -->

> Progress dihitung otomatis dari GitHub Project Kanban berdasarkan jumlah item berstatus `Done` dibandingkan total item yang memiliki field `Status`.

---

## 📞 Saluran Komunikasi Tim

| Kanal | Fungsi | Tautan |
|---|---|---|
| 💬 Teams | Diskusi formal dan koordinasi | [Buka Teams](#) |
| 📂 SharePoint | Penyimpanan dokumen kerja | [Buka SharePoint](#) |
| 🗂️ GitHub Project Kanban | Tasking dan tracking progres | [Buka Project](#) |
| 📱 WhatsApp | Koordinasi cepat | [Buka WA](#) |

---

## 📁 Struktur Folder Kerja

```text
0_Belajar Bareng/
├── 00_Admin/
├── D_Data/
│   ├── 1_Sekunder/
│   ├── 2_Prime/
│   ├── 3_Analisis/
│   ├── 4_Kobo/
│   └── Image/
├── P_Produk/
│   ├── P1_Laporan/
│   ├── P2 Peta/
│   └── P3_Dashboard/
└── Z_Arsip/
```

---

## 🧩 Format Tasking 8-Field

Setiap issue harus memakai format 8-field:

| Field | Isi |
|---|---|
| Apa | Tugas yang harus dikerjakan |
| Tujuan | Alasan tugas diperlukan |
| Hasil | Output akhir yang diharapkan |
| Format | Bentuk output (Excel, PDF, Markdown, Peta, Dashboard, Slide) |
| Prioritas | Tinggi / Sedang / Rendah |
| Deadline | Tanggal dan jam batas pengerjaan |
| Sumber Data / Referensi | Dataset, dokumen, tautan |
| Requester | Pihak yang meminta tugas |

---

## ⚙️ Integrasi Progress Otomatis

Blok ini akan diperbarui otomatis oleh workflow GitHub Actions:

```markdown
<!-- PROJECT_PROGRESS:START -->
![Progress](https://geps.dev/progress/0)
**Progress Kanban:** 0/0 item selesai (0%).
<!-- PROJECT_PROGRESS:END -->
```

Workflow menghitung:

```text
Progress = jumlah item Done ÷ total item dengan Status × 100
```

Status yang dihitung selesai: `Done`, `Selesai`, `Completed`, `Complete`.

---

## 📎 Dokumen Pendukung

- `CARA_PAKAI_PROGRESS.md` — Panduan workflow dan README progress
- `STRUKTUR_FOLDER.md` — Panduan penggunaan folder
- `LABEL_ISSUE.md` — Rekomendasi label GitHub Issue
- `tasking-8-field.md` — Template issue GitHub untuk 8-field tasking
