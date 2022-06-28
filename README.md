# Crack File Password using John The Ripper
使用John The Ripper破解檔案密碼。
* 暴力破解
* 字典檔

## **環境&工具**
* 系統：Kali Linux
* 一個加密的檔案
* 一個字典檔

## **搜尋Kali內建字典檔**
* 至`/usr/share/wordlists`路徑下，將rockyou.txt.gz解壓縮後得到rockyou.txt
  ```shell
  gunzip rockyou.txt.gz
  ```
  > ![image](https://github.com/WanShannn/Crack-File-Password-JohnTheRipper/blob/main/result/0.png)

## **攻擊**
* 指令
  ```shell
  john --wordlist=字典檔 --format=加密的格式 要破解的檔案
  ```
  > ![image](https://github.com/WanShannn/Crack-File-Password-JohnTheRipper/blob/main/result/1.png)

## **破解後**
* 以破解的檔案<font color="#f00">不接受再次破解</font>
* 破解完的內容將會存在 ~/.john/john.pot 裡面
* 把檔案john.pot內容清空即可再次破解
> ![image](https://github.com/WanShannn/Crack-File-Password-JohnTheRipper/blob/main/result/2-1.png)
> ![image](https://github.com/WanShannn/Crack-File-Password-JohnTheRipper/blob/main/result/2-2.png)
  
## **References**
* https://zh.wikipedia.org/zh-tw/John_The_Ripper
* https://hackercat.org/hacker-tools/john-the-ripper
* https://github.com/openwall/john
