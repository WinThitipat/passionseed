# Roboto Sans — Easy Solve

## 📝 Steps to Solve

### 1. Launch the instance
Click **“here”** to start the challenge.  
<img src="https://github.com/user-attachments/assets/1ce4ec8c-29f8-4d6d-b61a-a965a84bb4ff" width="600" />

---

### 2. Visit the website
A strange page appears.  
<img src="https://github.com/user-attachments/assets/e0e532c8-c5ec-444e-97d6-114345654ee1" width="600" />

---

### 3. Check `robots.txt`
Go to `/robots.txt` in the URL.  
<img src="https://github.com/user-attachments/assets/f2d63036-2860-457e-b850-9340b877cdc3" width="400" />

It shows:  
- Some hidden pages (`/cgi-bin/`, `/wp-admin/`)  
- A Base64 string  
<img width="619" height="335" alt="image" src="https://github.com/user-attachments/assets/c432f360-727d-4030-88a8-b5c42629a772" />

---

### 4. Test the hidden pages
- `/cgi-bin/` → locked  
- `/wp-admin/` → locked  

<img src="https://github.com/user-attachments/assets/5daf46aa-aeda-4c5f-9a54-eff7f3c51aa9" width="600" />  
<img src="https://github.com/user-attachments/assets/b6d571d2-8243-4c42-aeb1-e64a1295eb13" width="600" />

---

### 5. Decode the Base64
The string decodes into **two more URLs**.  
<img src="https://github.com/user-attachments/assets/f7a4d98b-6f57-4405-9ee9-c8b117e26c97" width="400" />

---

### 6. Try the decoded URLs
- First URL → invalid  
- Second URL → success ✅  

<img src="https://github.com/user-attachments/assets/104d6ff6-933e-40cf-9fcb-2eebf3c678d0" width="600" />  
<img src="https://github.com/user-attachments/assets/f8171a44-5065-4f45-addf-d03162900808" width="600" />

---

### 7. Get the flag 🎉
The second hidden page contains the **flag**.  

---

## ✅ Summary
1. Opened the website.  
2. Checked `/robots.txt`.  
3. Found Base64 → decoded it.  
4. Tested new URLs.  
5. One worked → revealed the flag!  

