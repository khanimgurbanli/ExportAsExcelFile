# Task
---- Azerbaijan -----


Lahiyə excel faylından məlumatları oxuyub məlumat bazasına yazmalıdır və dataya görə hesabatları email vasitəsi ilə göndərməlidir. Excel məlumatlarına uyğun nümuneden istifadə edərək məlumat bazası qurulur ve datalar orda saxlanılır.

Enpointler aşağıdaklar olmalıdır
UploadData/POST/File(binary) - məlumat faylı yüklənməsi - fayl yalnız xlxs və xls ola bilər, max 5mb yükləyə bilməlidir, yüklənmiş faylın template uyğun olması lazımdır.
SendReport/GET/Type(int) | StartDate(DateTime) | EndDate(DateTime) | AcceptorEmail(string[]) - hesabatın növü və email ünvanları göndərərək hesabat istəyi - Type enum olmalıdır və seçimlərin çölündə ola bilməz, emaillərin düzgün formatda bitiyini və code.edu.az domainə aid olduğunu yoxlamaq. StartDate-in EndDate-dən kiçik olduğunu yoxlamaq.
Hesabat növləri
1 - Segment-ə görə satışlar - Hər segmentə görə tarix aralığında məhsul sayı, satiş toplamı, endirim toplamı, qazanc toplamı məlumatları

2 - Ölkəyə görə satışlar - Hər ölkəyə görə tarix aralığında məhsul sayı, satiş toplamı, endirim toplamı, qazanc toplamı məlumatları

3 - Məhsula görə satışlar - Hər məhsula görə tarix aralığında məhsul sayı, satiş toplamı, endirim toplamı, qazanc toplamı məlumatları

4 - Məhsula görə endirimlər - Hər məhsula görə tarix aralığında məhsula necə faiz endirim olunduğu məlumat

 İstifadə olunan toollar
Code Coverage Summary
Logging
Sistemdə bütün əməliyyatlar və xətalar loglanmalıdır.
Hansı emaillərə hansi hesabatlar göndərilib loglanmalıdır.
Texnologiyalar
Backend : .NET, Java, Python
UI: SwaggerUI, Js
Database: SQL Server, PostgreSQL
Git: GitHub
Email Client: SendGrid

----English-----



The project should read the data from the excel file and write it to the database and send the reports based on the data via email. A database is created using a pattern corresponding to Excel data and the data is stored there.

Enpoints should be the following
UploadData/POST/File(binary) - data file upload - the file can only be xlxs and xls, it must be able to upload max 5mb, the uploaded file must match the template.
SendReport/GET/Type(int) | StartDate(DateTime) | EndDate(DateTime) | AcceptorEmail(string[]) - type of report and report request by sending email addresses - Type must be enum and cannot be outside the options, check that emails end in the correct format and belong to the code.edu.az domain. Checking if StartDate is less than EndDate.
Report types
1 - Sales by Segment - Number of products, sales total, discount total, profit total data in the date range for each segment

2 - Sales by country - Number of products, sales total, discount total, profit total data in the date range for each country

3 - Sales by product - Number of products, sales total, discount total, profit total data in the date range for each product

4 - Discounts by product - Information on how the product is discounted in the date range for each product

  Tools used
Code Coverage Summary
Logging
All operations and errors must be logged in the system.
What reports should be sent to which emails and logged.
Technologies
Backend: .NET, Java, Python
UI: SwaggerUI, Js
Database: SQL Server, PostgreSQL
Git: GitHub
Email Client: SendGrid
