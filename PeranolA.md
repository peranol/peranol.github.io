requirement ID : V1.2.4   
requirement Detail : Verify that all authentication pathways and identity management APIs implement consistent authentication security control strength, such that there are no weaker alternatives per the risk of the application.     
OTG # 1 :Test remember password functionality (OTG-AUTHN-005)  
        - รหัสผ่านในการจัดเก็บเบราว์เซอร์ไม่เพียงสะดวกสบายเท่านั้นสำหรับผู้ใช้งาน แต่ยังมีการสะสมอาวุธไปยังเบราว์เซอร์ของเหยื่อ (เช่นผ่าน Cross Site Scripting ทหารหรือผ่านคอมพิวเตอร์ที่ใช้ร่วมกัน) จากนั้นพวกเขาสามารถดึงข้อมูลรหัสผ่านที่เก็บไว้ไม่ใช่เรื่องแปลกที่เบราว์เซอร์จะจัดเก็บสิ่งเหล่านี้ รหัสผ่านในลักษณะที่ได้รับการเอาชนะอย่างเต็มที่ แต่เบราว์เซอร์ เพื่อจัดเก็บรหัสผ่านที่เข้ารหัสและเรียกคืนได้เท่านั้น ด้วยการใช้รหัสผ่านหลักผู้โจมตีสามารถเรียกดูได้รหัสผ่านโดยไปที่การตรวจสอบสิทธิ์ของแอปพลิเคชันเว็บเป้าหมายฟอร์มป้อนชื่อผู้ใช้ของเหยื่อและปล่อยให้เบราว์เซอร์เพื่อป้อนรหัสผ่าน  
OTG # 2 :Testing for Weak or unenforced username policy (OTG-IDENT-005)  
        - ชื่อบัญชีผู้ใช้มักจะมีโครงสร้างสูง (เช่น Joe Bloggs ชื่อบัญชีคือ jbloggs และ Fred Nurks ชื่อบัญชีคือ fnurks) และชื่อบัญชีที่ถูกต้องสามารถเดาได้ง่าย
