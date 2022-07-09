# SQL-Documentation

# Table Of Content
- [Veri Tabani Yonetim Sistemleri](#veri-tabani-yonetim-sistemleri)
- [Temel SQL Komutlari](#temel-sql-komutlari)
  * [Select](#select)
  * [Instert](#instert)
  * [Update](#update)
  * [Delete](#delete)
  * [Truncate](#truncate)
  * [Where](#where)
  * [AND](#and)
  * [OR](#or)
  * [DISTINCT](#distinct)
  * [ORDERBY](#orderby)
  * [GROUPBY](#groupby)
  * [TOP](#top)
- [Database Restore Etme Ornegi](#database-restore-etme-ornegi)


# Veri Tabani Yonetim Sistemleri
# Temel SQL Komutlari
## Select

    SELECT   
    KOLON1,KOLON2,KOLON3  
    FROM TABLOADI  
    WHERE <SARTLAR>  
    
![Screenshot from 2022-06-10 22-33-47](https://user-images.githubusercontent.com/57320216/173185530-987f2cf2-46f8-44e8-8af2-2ab3f44dce8b.png)  
![Screenshot from 2022-06-10 22-33-56](https://user-images.githubusercontent.com/57320216/173185531-13351a63-b0e7-4c79-96ed-9dafb98050c1.png)


## Instert

    INSERT INTO TABLOADI  
    (KOLON1,KOLON2,KOLON3)  
    VALUES  
    (VALUE1,VALUE2,VALUE3)    
![Screenshot from 2022-06-10 22-36-56](https://user-images.githubusercontent.com/57320216/173185603-53e5b2bd-ce31-4b4b-b03f-cdff64a672c4.png)   

##### Eğer verileriniz, csv, tsv, excell formatındaysa, veritabanına atmak için izlemeniz gereken pipeline : 

- Önce     
="insert into cars(marka,model,donanim,motor,yakit,vites,fiyat) VALUES('"&A2&"','"&B2&"','"&C2&"','"&D2&"','"&E2&"','"&F2&"','"&G2&"')   
formülü kullanılarak sutündaki veriler çekilir.  
![Screenshot from 2022-07-09 21-22-43](https://user-images.githubusercontent.com/57320216/178122175-1f1eaadd-be18-458e-9391-28196baf927d.png)
![Screenshot from 2022-07-09 21-27-36](https://user-images.githubusercontent.com/57320216/178122179-ea58b18b-9b34-44f4-ab2e-865d56a60731.png)

- Çekilen veri son satıra kadar çekilir ve diğer satırların da otomatik doldurulması sağlanır.  
![Screenshot from 2022-07-09 21-29-02](https://user-images.githubusercontent.com/57320216/178121968-b2657876-7f1a-4064-8344-4bbd88ec4a1e.png)

- En son tüm komutlar kopyalanarak veritabanına eklenir.
![Screenshot from 2022-07-09 22-01-40](https://user-images.githubusercontent.com/57320216/178122099-f13ae170-7963-4e9c-b97d-7336ac2bf585.png)
![Screenshot from 2022-07-09 22-44-28](https://user-images.githubusercontent.com/57320216/178122103-9368c710-fbac-4d19-8f9d-cf20ad99248c.png)  
Yeni veritabanımızı oluşmuş oldu. Şimdi veritabanında nasıl veri set edilip, güncellenebilir. 

## Update

    UPDATE TABLENAME  
    SET COLUMN1=VALUE1,COLUMN2=VALUE2....,  
    WHERE <ŞARTLAR>  
    
    SELECT * FROM cars
    UPDATE cars
    set motor ='

![Screenshot from 2022-07-09 22-47-45](https://user-images.githubusercontent.com/57320216/178122268-107efaee-0668-4293-bd2a-af20ec0b5166.png)
![Screenshot from 2022-07-09 22-48-35](https://user-images.githubusercontent.com/57320216/178122270-8ae88343-f587-4cca-9de4-2d43de24ee32.png)
![Screenshot from 2022-07-09 22-48-47](https://user-images.githubusercontent.com/57320216/178122272-700429db-41ea-45f6-8a47-746399eb505a.png)
![Screenshot from 2022-07-09 22-50-16](https://user-images.githubusercontent.com/57320216/178122274-6afbc963-3880-49d2-a5cb-42d3aefcbbaa.png)


## Delete

    DELETE
    FROM TABLENAME
    WHERE <ŞARTLAR>

 
## Truncate 

    TRUNCATE TABLE TABLENAME
    
 İlk haline dönüştürür. Delete hepsini siler. Hız; Truncate >> Delete
 Delete de otomatk artan bir alan varsa (ID) gibi en son kaldığı yerden devam eder. Truncate 0lar.

## Where
## AND
## OR 
## DISTINCT
## ORDERBY
## GROUPBY
## TOP
# Database Restore Etme Ornegi

