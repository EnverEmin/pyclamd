import pyclamd

# ClamAV bağlantısını aç
cd = pyclamd.ClamdAgnostic()

# Bilgisayarı tarayın
scan_result = cd.scan_recursive('/')

# Eğer bir virüs bulunursa, virüs adını yazdırın
if scan_result is not None:
  for file_name, virus_name in scan_result.items():
    print(f'{file_name} dosyasında {virus_name} virüsü bulundu.')
