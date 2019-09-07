HTML Injection (POST)  
member :  
Ardnarong Boonkerd  
Suparath Suwannakorth  
Peranol Akkarasarateera  
  <p align="center">
    <img src="PIC/bWAPP - HTML Injection.png">
  </p>

-ทดสอบช่องโหว่ด้วยการ input html code
-test<img src="http://192.168.43.95/bWAPP/images/blogger.png" />
-ลงทั้ง 2 ช่อง input
  <p align="center">
    <img src="PIC/bWAPP - HTML Injection (1).png">
  </p>

-จากนั้นระบบจะแสดงตามรูป  
-

-แสดงว่าสามารถทำ html injection ได้ทั้ง 2 input  
-วิธีการแก้ไข   
- download code ชื่อ htmli_post.php โดยใช้  winscp  login ด้วย user : bob/password : bob456  
-

-จากนั้นเปิดไฟล์ เพื่อแก้ไข code พบว่าไม่มีการ validation ตัวแปร firstname + lastname
-

-ในการแก้ไขสามารถใช้ function อื่น ได้แก่ strip_tags เป็นต้น  
-จากนั้นทำการ rename จาก htmli_post.php เป็น htmli_post_bob.php
-แล้วทำการ upload htmli_post_bob.php ขึ้น server


