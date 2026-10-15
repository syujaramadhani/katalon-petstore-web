# Katalon Petstore Web

Project web automation pakai Katalon Studio untuk https://petstore.octoperf.com/actions/Catalog.action

## Cara menjalankan
1. Buka project ini di Katalon Studio (File > Open Project).
2. Buka Test Suites > TS_Petstore_Regression.
3. Pilih browser Chrome, lalu klik Run.
4. Report ada di folder Reports. Contoh hasil run ada di folder execution-report.

Kalau error ChromeDriver, update dulu lewat Tools > Update WebDriver.

## Global Variable
URL, username, dan password ada di Profiles/default.glbl (BASE_URL, USERNAME, PASSWORD).
Akun yang dipakai adalah akun demo bawaan website petstore.

## Test Suite
TS_Petstore_Regression, isinya semua test case di bawah.

## Test Case
| Test Case | Jenis | Keterangan |
|---|---|---|
| TC01_Login_Valid | Positive | Login pakai username dan password dari Global Variable |
| TC02_Login_Invalid | Negative | Login dengan data salah dari Data Files/login_data.csv (DDT) |
| TC03_Search_Bulldog | Positive | Cari produk bulldog |
| TC04_Search_NotFound | Negative | Cari keyword yang tidak ada |
| TC05_AddToCart_Bulldog | Positive | Tambah bulldog ke cart |
