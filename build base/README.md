
# Info Negara

Library Info Negara adalah modul Python yang dirancang untuk berinteraksi dengan REST Countries API. Modul ini menyediakan antarmuka sederhana melalui class libraryNegara untuk mendapatkan informasi penting tentang suatu negara. Dengan memanfaatkan modul requests, library ini mempermudah akses informasi seperti nama negara, ibu kota, mata uang, dan populasi, sehingga memudahkan pengembang untuk mengintegrasikannya ke dalam aplikasi mereka.


## API 

#### Python Basic API wrapper

```http
  https://restcountries.com/v2/
```
## Installation

Install my-project with npm

```bash
  pip install infonegara
```
    
## Usage
Basic Usage:

```javascript
from info_negara import libraryNegara

library_negara = libraryNegara()

nama_negara = input("Masukkan nama negara dengan bahasa inggris: ")
info_negara = library_negara.get_info_negara(nama_negara)

if info_negara:
    print("\nInformasi Negara")
    print(f"Nama Negara: {info_negara.nama}")
    print(f"Ibu Kota: {info_negara.ibukota}")
    print(f"Mata Uang: {info_negara.matauang}")
    print(f"Jumlah Penduduk: {info_negara.populasi}")
    print("")
else:
    print(f"Negara '{nama_negara}' tidak ditemukan.")
    
```

