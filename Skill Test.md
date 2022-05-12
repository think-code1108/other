# Skill Test

## Soal
Buatlah sebuah aplikasi web sederhana menggunakan bahasa pemograman yang anda kuasai, aplikasi tersebut memiliki Layar:
 * Layar List (untuk view data), berisi informasi list data dari API berikut:
    * API:
      ```
      Method: POST
      URL: https://service.jec.co.id/api/jec_api/JSONFAKE/TestDataPasien
      body:
      {
          "token": "XQ39pdVh",
          "ClinicName": "JEC@CORP",
          "mode": "getdata"
      }
    * Return API:
      ```
      {
      "result": "success",
      "data": [
          {
            "ID": 1,
            "FirstName": "Zico",
            "MiddleName": "",
            "LastName": "Alamsyah",
            "BirthDate": "17-08-1990",
            "Gender": "Male"
          },
          {
            "ID": 3,
            "FirstName": "Teguf",
            "MiddleName": "Adi",
            "LastName": "Wibowo",
            "BirthDate": "17-08-1990",
            "Gender": "Male"
          }
        ]
      }
  
 * Layar Add, Edit dan Delete Data, Berisi Form data dari atribut data pasien, yaitu FirstName, MiddleName, LastName, Birthdate dan Gender. Berikut APInya:
    * API (Add / Insert):
      ```
      Method: POST
      URL: https://service.jec.co.id/api/jec_api/JSONFAKE/TestDataPasien
      body:
      {
          "token": "XQ39pdVh",
          "ClinicName": "JEC@CORP",
          "mode": "insertdata",
          "FirstName": "Rio",
          "MiddleName": "Adi",
          "LastName": "Manurung",
          "BirthDate": "19900810",
          "Gender": "Male"
      }
    * Return API (Add / Insert):
      ```
      {
        "result": "success",
        "data": [
            {
              "Message": "Insert data Succeed"
            }
        ]
      }

    * API (Edit / Update):
      ```
      Method: POST
      URL: https://service.jec.co.id/api/jec_api/JSONFAKE/TestDataPasien
      body:
      {
          "token": "XQ39pdVh",
          "ClinicName": "JEC@CORP",
          "mode": "updatedata",
          "FirstName": "Rio",
          "MiddleName": "Andi",
          "LastName": "Manurung",
          "BirthDate": "19900810",
          "Gender": "Male",
          "id": 7
      }
    * Return API (Edit / Update):
      ```
      {
        "result": "success",
        "data": [
            {
              "Message": "Update data Succeed"
            }
        ]
      }

    * API (Delete):
      ```
      Method: POST
      URL: https://service.jec.co.id/api/jec_api/JSONFAKE/TestDataPasien
      body:
      {
          "token": "XQ39pdVh",
          "ClinicName": "JEC@CORP",
          "mode": "deletedata",
          "id": 7
      }
    * Return API (Delete):
      ```
      {
        "result": "success",
        "data": [
            {
              "Message": "Delete data Succeed"
            }
        ]
      }
      
      
# Selamat Mengerjakan
