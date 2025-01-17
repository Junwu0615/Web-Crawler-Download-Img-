<a href='https://github.com/Junwu0615/Web-Crawler-Download-Img'><img alt='GitHub Views' src='https://views.whatilearened.today/views/github/Junwu0615/Web-Crawler-Download-Img.svg'> 
<a href='https://github.com/Junwu0615/Web-Crawler-Download-Img'><img alt='GitHub Clones' src='https://img.shields.io/badge/dynamic/json?color=success&label=Clone&query=count_total&url=https://gist.githubusercontent.com/Junwu0615/706da0097d75deeae8342f2203db8b19/raw/Web-Crawler-Download-Img_clone.json&logo=github'> </br>
[![](https://img.shields.io/badge/Project-Web_Crawler-blue.svg?style=plastic)](https://github.com/Junwu0615/Crawler-Keywords-And-Use-LineBot) 
[![](https://img.shields.io/badge/Language-Python_3.12.0-blue.svg?style=plastic)](https://www.python.org/) </br>
[![](https://img.shields.io/badge/Package-BeautifulSoup_4.12.2-green.svg?style=plastic)](https://pypi.org/project/beautifulsoup4/) 
[![](https://img.shields.io/badge/Package-Requests_2.31.0-green.svg?style=plastic)](https://pypi.org/project/requests/) 
[![](https://img.shields.io/badge/Package-ArgumentParser_1.2.1-green.svg?style=plastic)](https://pypi.org/project/argumentparser/) 

## STEP1.　CLONE
```py
git clone https://github.com/Junwu0615/Web-Crawler-Download-Img.git
```

## STEP.2　INSTALL PACKAGES
```py
pip install -r requirements.txt
```

## STEP3.　RUN
```py
python Entry.py -h
```

#### If you encounter the following problems :
> ModuleNotFoundError: No module named 'python'.<br/>
> ModuleNotFoundError: No module named 'pip'. 
1. 去檢查 C:\Users\xxx\AppData\Local\Programs\Python 是否有檔案。
1. 若無，則去 [Python](https://www.python.org/downloads/) 官網下載並安裝。
1. 接著再次執行該指令；若一樣出現同樣錯誤，去 `系統環境變數` 當中新增 `2` 個路徑 ( Path ) 即可 :
    - C:\Users\ `xxx` \AppData\Local\Programs\Python\ `Python版本`
    - C:\Users\ `xxx` \AppData\Local\Programs\Python\ `Python版本` \Scripts

## STEP4.　HELP

- `-h` Help:　Show this help message and exit.
- `-t` Type:　Give a type of websites | ex:　[Unsplash](https://unsplash.com/) / [Ptt](https://www.ptt.cc/bbs/Beauty/index.html) / [Google Picture](https://www.google.com/imghp?hl=zh-TW&ogbl)
- `-u` Url :　 Give a url | ex:　https://...
- `-p` Path:　Give a path | ex:　./img

## STEP5.　EXAMPLE
#### python Entry.py `-t 類型` `-u 網址` `-p 儲存路徑` ，共 3 個輸入內容，具體請參考 `STEP3. HELP`。<br/>
#### 當網址太長時，可以使用 [PicSee 縮短網址](https://picsee.io/?utm_source=picsee-co&utm_medium=referral&utm_term=home) 來幫助 `命令提示字元(cmd)` 讀取，以避免出錯。<br/><br/>

### I.　PTT Beauty 版下載圖片
在 **PTT Beauty版** 搜尋內容並點選進入後，其網址即為 `-u` ，並將圖片存放於 **./downloads**。
- `-t` PTT
- `-u` https://www.ptt.cc/bbs/Beauty/M.1702040877.A.239.html
- `-p` ./downloads
```py
python Entry.py -t ptt -u https://www.ptt.cc/bbs/Beauty/M.1702040877.A.239.html -p ./downloads
```
![森香澄.gif](/sample/森香澄.gif)
 - 運行完畢後會在 `./downloads` 生成多個 `jpg` 檔。
 - 森香澄.jpg
 - ![森香澄.jpg](/sample/森香澄.jpg)

<br/>

### II.　Unsplash 下載圖片
在 **Unsplash** 以關鍵字 **cat** 搜尋後，其網址即為 `-u` ，並將圖片存放於 **./downloads**。
- `-t` unsplash
- `-u` https://unsplash.com/s/photos/cat
- `-p` ./downloads
```py
python Entry.py -t unsplash -u https://unsplash.com/s/photos/cat -p ./downloads
```
 - 運行完畢後會在 `./downloads` 生成多個 `jpg` 檔。
 - cat12.jpg
 - <img width='426' height='640' src="https://github.com/Junwu0615/Web-Crawler-Download-Img/blob/master/sample/cat12.jpg"/>


## 參考來源
- [STEAM 教育學習網 | 爬取後同時下載多張圖片](https://steam.oxxostudio.tw/)
