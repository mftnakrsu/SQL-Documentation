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

![Screenshot from 2022-07-09 21-22-43](https://user-images.githubusercontent.com/57320216/178121962-a0f0ceb1-1930-42d5-9625-a2914ac1bf86.png)
- Çekilen veri son satıra kadar çekilir ve diğer satırların da otomatik doldurulması sağlanır.  
![Screenshot from 2022-07-09 21-27-36](https://user-images.githubusercontent.com/57320216/178121964-4918f70f-0b28-4c75-ad65-868707386019.png)
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


## Delete
## Truncate 
## Where
## AND
## OR 
## DISTINCT
## ORDERBY
## GROUPBY
## TOP
# Database Restore Etme Ornegi

