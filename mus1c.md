# mus1c — Easy Solve

## 🎵 Challenge Walkthrough

### 1. Download the file
<img src="https://github.com/user-attachments/assets/6bbdd4d7-55f6-4d84-ab71-57924eca5d93" width="700" />

---

### 2. Analyze the content
When opening the file, we get some *weird song lyrics*.  
It looks like some kind of pseudo-code hidden inside the music text.

Example snippet:

Pico's a CTFFFFFFF
my mind is waitin
It's waitin

Put my mind of Pico into This
my flag is not found
put This into my flag
put my flag into Pico


shout Pico
shout Pico
shout Pico

My song's something
put Pico into This

Knock This down, down, down
put This into CTF

shout CTF
my lyric is nothing
Put This without my song into my lyric
Knock my lyric down, down, down

shout my lyric

Put my lyric into This
Put my song with This into my lyric
Knock my lyric down

shout my lyric

Build my lyric up, up ,up

shout my lyric
shout Pico
shout It

Pico CTF is fun
security is important
Fun is fun
Put security with fun into Pico CTF
Build Fun up
shout fun times Pico CTF
put fun times Pico CTF into my song

build it up

shout it
shout it

build it up, up
shout it
shout Pico


---

### 3. Hint → Rockstar language
The challenge hint mentioned **Rockstar**.  
After searching, we found out that [Rockstar](https://github.com/RockstarLang/rockstar) is a joke programming language where code is written in the style of 1980s rock lyrics. 🎸

<img src="https://github.com/user-attachments/assets/819201d3-c958-48e4-955f-cd710962284a" width="700" />

---

### 4. Run the lyrics as Rockstar code
By pasting the lyrics into a Rockstar interpreter, the program executes successfully.

<img src="https://github.com/user-attachments/assets/5e4567c2-aaa8-4270-b106-f6f5dc85893b" width="400" />

---

### 5. Check the output
The output looks like **ASCII values**.

<img src="https://github.com/user-attachments/assets/4d68c6a9-6a6a-413a-92cb-05e2c391401d" width="600" />

---

### 6. Convert ASCII → Text
We decode the ASCII numbers into text (UTF-8).  
This gives us the hidden message.

<img src="https://github.com/user-attachments/assets/c4e61632-ceb7-4c02-8c2c-5dd088ab1085" width="700" />

---

### 7. Construct the flag
Finally, we wrap the decoded message with `picoCTF{}` format.  
That gives us the correct flag ✅

<img src="https://github.com/user-attachments/assets/178ad8d7-9c05-42d3-abc2-0f5e409baf95" width="700" />

---

## 🎯 Summary
- The file was actually **Rockstar source code** disguised as song lyrics.  
- Running it in a Rockstar interpreter produced ASCII codes.  
- Converting those codes to text revealed the hidden message.  
- Wrapping it with `picoCTF{}` gave the final flag 🎉  
