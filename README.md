## Tentang repo ini

Repo ini digunakan untuk menulis resensi tentang pemenang Hadiah Nobel Ekonomi 2026, Hall dan Woodford. Isinya:

- `nobel2026-paper.qmd`: policy brief.
- `nobel2026-deck.qmd`: presentasi (beamer PDF dan revealjs HTML).

Hasil render tersimpan di folder `docs/`.

Alur tulisan (berlaku untuk paper maupun deck):

1. Pendahuluan
2. Kontribusi Hall dan Woodford
3. Relevansinya bagi Indonesia

## Cara menggunakan

### Kebutuhan

- [Quarto](https://quarto.org)
- Distribusi LaTeX dengan `lualatex` (misalnya TeX Live atau TinyTeX: `quarto install tinytex`)

### Mengedit policy brief

1. Buka `nobel2026-paper.qmd`.
2. Ubah judul, penulis, abstrak, dan kata kunci di bagian YAML (di antara tanda `---` di awal file).
3. Tulis isi tulisan di bawah YAML menggunakan Markdown.
4. Tambahkan referensi ke `ref.bib`, lalu kutip dengan `@kunci` (misalnya `@hall1978`).

### Mengedit presentasi

1. Buka `nobel2026-deck.qmd`.
2. Ubah judul dan tanggal di bagian YAML.
3. Setiap judul `##` menjadi satu slide baru. Kelas yang tersedia, misalnya `{.small}`, `{.smaller}`, `{.section-divider}`, dan `{.ending-slide}`, sudah dicontohkan di dalam file.

### Render

Dari folder repo, jalankan:

```bash
quarto render                          # render paper dan deck
quarto render nobel2026-paper.qmd      # render paper saja
quarto render nobel2026-deck.qmd       # render deck saja
```

Hasilnya akan muncul di folder `docs/`.

## Sitasi

Sitasi yang dapat digunakan adalah:

Last, First. year. paper name. DEN Working Paper no. x.

atau jika anda menggunakan bibtex:

```bibtex
@article{citekey,
  author  = {Nash, John},
  title   = {Non-cooperative Games},
  journal = {DEN Working Paper},
  year    = {2026},
  volume  = {3},
  url = {}
}
```

## Lisensi dan Hak Cipta
Seluruh aset, kode, dan data dalam repositori ini dilindungi di bawah **Lisensi DEN**.

Penggunaan, penggandaan, atau pendistribusian materi di dalam repositori ini harus mematuhi ketentuan yang tercantum dalam file **[LICENSE](LICENSE)**.

*Hak Cipta (c) 2026 Dewan Ekonomi Nasional Republik Indonesia (DEN)*
