# FHCTF write up

## imformation
老樣子，先dirsearch一下，就發現了熟悉的redoc，原來是API又沒鎖(好像跟某間學校一樣哈哈)

![alt text](image-11.png)
![alt text](image.png)

在API裡的getflag就有flag的網址了

![alt text](image-1.png)
![alt text](image-2.png)
## A web
老樣子，先dirsearch一下，就去看看robot.txt，找到第一段

![alt text](image-12.png)
![alt text](image-3.png)

用XSS找到第二段

![alt text](image-4.png)
![alt text](image-5.png)

第三段來不及找，有看到isadmin這個參數，估計是從其下手

## 時空呂人
提示說在flag.txt，所以就想辦法找出他

![alt text](image-6.png)
![alt text](image-7.png)

參考:https://medium.com/@Aftab700/nginx-configuration-wizer-ctf-88c47f61aa2b
## 上鎖了！？
老樣子，先dirsearch一下

![alt text](image-13.png)

robot.txt是騙人的，就去admin看看

![alt text](image-8.png)
反白之後就看到酷東西

![alt text](image-14.png)

但是權限不足，我個人猜想是要改cookie讓自己變成admin進去

![alt text](image-10.png)