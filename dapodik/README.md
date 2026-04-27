# Indonesia School Data Snapshot

This repository contains a **snapshot of publicly accessible education data** collected from official Indonesian Ministry of Education portals which then was:

* [https://dapo.kemdikbud.go.id](https://dapo.kemdikbud.go.id)
* [https://referensi.data.kemdikbud.go.id](https://referensi.data.kemdikbud.go.id)


## Overview

The datasets originate from:
* **Dapodik (Data Pokok Pendidikan)** — national system for education data (schools, students, teachers, infrastructure)
* **Referensi Data Kemdikbud** — master/reference datasets used across education systems

collected in November 2023. This repository serves as a **static data archive** for research, analysis, and reproducibility of results based on that time period. _This repository only redistributes transformed public data._

## What’s Included

### From Dapodik (Data Pokok Pendidikan)

#### Profil Sekolah

* kecamatan
* kabupaten
* propinsi
* kode_kecamatan
* kode_kab
* kode_prop
* nama_sekolah
* npsn
* alamat_jalan
* status (negeri/swasta)

#### Rekapitulasi

* Data PTK dan PD
    * semester_id
    * rombel
    * guru_kelas
    * guru_matematika
    * guru_bahasa_indonesia
    * guru_bahasa_inggris
    * guru_sejarah_indonesia
    * guru_pkn
    * guru_penjaskes
    * guru_agama_budi_pekerti
    * guru_seni_budaya
    * ptk_laki
    * ptk_perempuan
    * pegawai_laki
    * pegawai_perempuan
    * pd_kelas_1_laki
    * pd_kelas_1_perempuan
    * pd_kelas_2_laki
    * pd_kelas_2_perempuan
    * pd_kelas_3_laki
    * pd_kelas_3_perempuan
    * pd_kelas_4_laki
    * pd_kelas_4_perempuan
    * pd_kelas_5_laki
    * pd_kelas_5_perempuan
    * pd_kelas_6_laki
    * pd_kelas_6_perempuan
    * pd_kelas_7_laki
    * pd_kelas_7_perempuan
    * pd_kelas_8_laki
    * pd_kelas_8_perempuan
    * pd_kelas_9_laki
    * pd_kelas_9_perempuan
    * pd_kelas_10_laki
    * pd_kelas_10_perempuan
    * pd_kelas_11_laki
    * pd_kelas_11_perempuan
    * pd_kelas_12_laki
    * pd_kelas_12_perempuan
    * pd_kelas_13_laki
    * pd_kelas_13_perempuan
    * jumlah_kirim
    * ptk
    * pegawai
    * pd
    * pd_laki
    * pd_perempuan

* Data Sarpras
    * before_ruang_kelas
    * after_ruang_kelas
    * before_ruang_perpus
    * after_ruang_perpus
    * before_ruang_lab
    * after_ruang_lab
    * before_ruang_praktik
    * after_ruang_praktik
    * before_ruang_pimpinan
    * after_ruang_pimpinan
    * before_ruang_guru
    * after_ruang_guru
    * before_ruang_ibadah
    * after_ruang_ibadah
    * before_ruang_uks
    * after_ruang_uks
    * before_toilet
    * after_toilet
    * before_gudang
    * after_gudang
    * before_ruang_sirkulasi
    * after_ruang_sirkulasi
    * before_tempat_bermain_olahraga
    * after_tempat_bermain_olahraga
    * before_ruang_tu	after_ruang_tu
    * before_ruang_konseling
    * after_ruang_konseling
    * before_ruang_osis
    * after_ruang_osis
    * before_bangunan
    * after_bangunan
    * identitas_valid
    * ptk_valid
    * pd_valid
    * prasarana_valid
    * total_valid

* Data Sanitasi
    * sekolah_id
    * sumber_air
    * sumber_air_minum
    * kecukupan_air_bersih
    * jamban_kk
    * tipe_jamban
    * jml_hari_cuci_tangan
    * jml_wastafel
    * jml_wastafel_rusak
    * air_mengalir_wastafel
    * memiliki_drainase
    * menguras_tangki_septik

### From Referensi Data Kemdikbud

* Identitas Satuan Pendidikan
    * Nama
    * NPSN
    * Alamat
    * Desa/Kelurahan
    * Kecamatan/Kota (LN)
    * Kab.-Kota/Negara (LN)
    * Propinsi/Luar Negeri (LN)
    * Status Sekolah
    * Bentuk Pendidikan

* Dokumen dan Perijinan
    * Kementerian Pembina
    * Naungan
    * NPYP
    * No. SK. Pendirian
    * Tanggal SK. Pendirian
    * Nomor SK Operasional
    * Tanggal SK Operasional
    * File SK Operasional
    * Tanggal Upload SK Op.
    * Akreditasi

* Sarana dan Prasarana
    * Luas Tanah
    * Akses Internet	
    * Sumber Listrik
    * Fax
    * Telepon
    * Email
    * Website

* Peta
    * Lintang
    * Bujur

## Data Source & Collection Methodology

The data in this repository was obtained by accessing publicly available endpoints of the official platforms listed above. The collection process relies on direct HTTP requests to endpoints that return structured JSON responses.

These endpoints are used internally by the websites to dynamically load data. By inspecting network activity (e.g., via browser developer tools), request URLs can be identified that return structured JSON payloads.

Key characteristics of the method:

* Requests are sent to publicly accessible URLs
* Responses are received in JSON format
* No authentication bypass or restricted access techniques were used
* No interaction with private or protected endpoints
* No HTML scraping or DOM parsing involved

**Note:**
The exact request patterns, scripts, or tooling used to collect the data are not included in this repository.

## Limitations

* Data completeness depends on what was publicly accessible at the time (~Nov 2023)
* Possible inconsistencies or missing values
* Some fields may have been normalized or reformatted
* The source websites are dynamic and may have changed since collection

## Disclaimer

* All data originates from publicly accessible government sources
* This repository is **not an official publication**
* The data is redistributed for:
    * Research
    * Educational use
    * Non-commercial analysis

## Suggested Use Cases

This dataset can support a wide range of analytical and practical applications, including:

* **Education Policy Analysis**: Evaluate distribution of teachers, students, and facilities across regions to support policy-making.
* **Geographic Visualization**: Build interactive maps of schools using geolocation data, including overlays for infrastructure and sanitation.
* **School Profiling & Benchmarking**: Compare schools based on student-teacher ratios, facility completeness, or infrastructure quality.
* **Infrastructure & Sanitation Assessment**: Identify gaps in sanitation and facilities across regions for targeted intervention or funding allocation.
* **Data Journalism & Public Transparency**: Create dashboards or visual stories highlighting disparities or trends in Indonesia’s education system.