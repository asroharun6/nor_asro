# Nor Asro

**Nor Asro** adalah library Python untuk normalisasi teks dalam bahasa Indonesia. Library ini dirancang untuk membantu membersihkan teks dengan cara mengganti kata slang menjadi formal, menghapus noise, dan melakukan stemming menggunakan Sastrawi.

## Fitur

- Normalisasi kata slang ke kata formal
- Mendukung file Excel untuk memuat daftar slang-formal
- Penghapusan noise seperti URL, angka, dan tanda baca
- Stemming untuk mendapatkan kata dasar

## Instalasi

```bash
pip install nor_asro


from nor_asro.normalizer import NorAsroNormalizer

# Inisialisasi normalizer dengan file Excel
normalizer = NorAsroNormalizer("path_to_your_excel_file.xlsx")

# Contoh teks
text = "Woww amin keberpa netaas met ya!"
result = normalizer.normalize_text(text)
print(result)  # Output: "wow amin keberapa menetas selamat ya"
