# Introduction to Git and GitHub

## Simple Interest Calculator (Kalkulator Bunga Sederhana)

A calculator that calculates simple interest given principal, annual rate of interest and time period in years.
Kalkulator yang menghitung bunga sederhana berdasarkan pokok (principal), suku bunga tahunan (annual rate of interest), dan periode waktu dalam tahun (time period in years).

### Rincian & Deskripsi Proyek / Project Details
Kalkulator bunga sederhana ini diimplementasikan menggunakan skrip Bash (`simple-interest.sh`). Program ini dirancang untuk menghitung jumlah bunga sederhana berdasarkan input pengguna secara interaktif melalui terminal dengan cepat dan akurat.

### Kolom Input / Input Fields
* **p (Principal amount / Pokok):** Jumlah modal awal atau pokok pinjaman/investasi yang diberikan.
* **r (Annual rate of interest / Suku bunga tahunan):** Tingkat suku bunga per tahun (dalam persen).
* **t (Time period in years / Periode waktu):** Jangka waktu investasi atau pinjaman dalam satuan tahun.

### Rumus Perhitungan / Formula
Bunga sederhana (Simple Interest) dihitung menggunakan rumus:
$$\text{Simple Interest} = \frac{p \times t \times r}{100}$$

```
Input:
   p, principal amount
   t, time period in years
   r, annual rate of interest

Output:
   simple interest = (p * t * r) / 100
```

### Cara Kerja Kalkulator / How it Works
1. Skrip meminta pengguna memasukkan jumlah pokok (`p`) melalui perintah `read p`.
2. Skrip meminta pengguna memasukkan suku bunga per tahun (`r`) melalui perintah `read r`.
3. Skrip meminta pengguna memasukkan jangka waktu dalam tahun (`t`) melalui perintah `read t`.
4. Skrip melakukan perhitungan aritmatika menggunakan perintah Bash:
   `s=$(expr $p \* $t \* $r / 100)`
5. Skrip menampilkan hasil perhitungan bunga sederhana (`s`) ke layar pengguna.

### Contoh Penggunaan / Example Usage
Misalkan seorang pengguna ingin menghitung bunga sederhana dengan rincian:
* Pokok (`p`) = 1000
* Suku bunga per tahun (`r`) = 5%
* Periode waktu (`t`) = 2 tahun

Perhitungan matematis:
$$\text{Simple Interest} = \frac{1000 \times 2 \times 5}{100} = 100$$

Contoh eksekusi di terminal:
```bash
$ bash simple-interest.sh
Enter the principal:
1000
Enter rate of interest per year:
5
Enter time period in years:
2
The simple interest is: 
100
```

_© 2023 XYZ, Inc._
