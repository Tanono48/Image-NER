# Image-NER
I modified it so that it skip GDrive mount part for the simplicity 

Hackathon link: https://www.kaggle.com/competitions/superai-hackathon-online-image-ner

ขั้นตอน OCR ดังนี้
1) ลดnoise ด้วย fastNmean 
2) ปรับ Gray scale 
3) ปรับรูปให้ตรงด้วย Deskew 
4) duplicate รูป ไว้ทำ edge detection 
5) gaussian blur 
6) ปรับ binary ด้วย OTSU 
7) Erode ทำเพิ่มให้เป็นเนื้อเดียว 
8) findContours  จับทีละคำ 
9) conV2D kernel sharp ให้ขอบตัวอักษรคม 
10) ใช้ tesseract
