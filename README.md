# **Repository Data Wrangling**
---

- Merupakan repository Data Wrangling yang digunakan Thread Twitter Pacmann (link soon...)
- Feel free yang ingin menggunakan repository ini untuk belajar
- Proses Data Wrangling yang dilakukan adalah:
    - Drop kolom `Unnamed: 0` karena tidak dibutuhkan
    - Remove `dot (.)` value pada kolom `rental_id`
    - Melakukan proses Mapping Values pada kolom `rental_status`. Kolom yang di mapping adalah:
        - `Overdue` menjadi `Late`
        - `Returns` menjadi `Returned`
    - Extract `Year` dan `Month` pada kolom `rental_date`. Tetapi kolom tersebut perlu di convert menjadi `datetime` terlebih dahulu dengan cara `pd.to_datetime(data)`
    - Filter data ke masing - masing status pada `rental_status`:
        - `Late`
        - `Rented`
        - `Returned`

    - Setelah itu simpan ke dalam bentuk csv:
        - `rental_late_data.csv`
        - `rental_rented_data.csv`
        - `rental_returned_data.csv`

Tabik

Tepe