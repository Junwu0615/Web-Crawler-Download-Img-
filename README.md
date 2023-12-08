[![](https://img.shields.io/badge/Project-Crawler-blue.svg?style=plastic)](https://github.com/Junwu0615/Crawler-Keywords-And-Use-LineBot) 
[![](https://img.shields.io/badge/Language-Python-blue.svg?style=plastic)](https://www.python.org/) </br>
[![](https://img.shields.io/badge/Package-BeautifulSoup-green.svg?style=plastic)](https://pypi.org/project/beautifulsoup4/) 
[![](https://img.shields.io/badge/Package-Requests-green.svg?style=plastic)](https://pypi.org/project/requests/) 
[![](https://img.shields.io/badge/Package-ThreadPoolExecutor-green.svg?style=plastic)](https://pypi.org/project/futures/) 
[![](https://img.shields.io/badge/Package-ArgumentParser-green.svg?style=plastic)](https://pypi.org/project/argumentparser/) 

## STEP1.　CLONE
```
git clone https://github.com/Junwu0615/Web-Crawler-Download-Img.git
```

## STEP2.　RUN
```
python download_multi_img.py -h
```
#若遇到以下問題 :
> ModuleNotFoundError: No module named 'python'.<br/>
> ModuleNotFoundError: No module named 'pip'. 
1. 去檢查 C:\Users\xxx\AppData\Local\Programs\Python 是否有檔案。
1. 若無，則去 [Python](https://www.python.org/downloads/) 官網下載並安裝。
1. 接著再次執行該指令；若一樣出現同樣錯誤，去 `系統環境變數` 當中新增 `2` 個路徑 ( Path ) 即可 :
    - C:\Users\ `xxx` \AppData\Local\Programs\Python\ `Python版本`
    - C:\Users\ `xxx` \AppData\Local\Programs\Python\ `Python版本` \Scripts
> ModuleNotFoundError: No module named 'bs4'.<br/>
  - `pip install beautifulsoup4`<br/>
> ModuleNotFoundError: No module named 'requests'.<br/>
  - `pip install requests`

## STEP3.　HELP
- -h　Help:　Show this help message and exit.
- -t　Type:　Give a type of web | ex:　[Unsplash](https://unsplash.com/) / [Ptt](https://www.ptt.cc/bbs/Beauty/index.html) / [Google Picture](https://www.google.com/imghp?hl=zh-TW&ogbl)
- -u　Url :　 Give a url | ex:　https://...
- -p　Path:　Give a path | ex:　./img

## STEP4.　EXAMPLE
#python download_multi_img.py `-t 類型` `-u 網址` `-p 儲存路徑` ，3個值能使用的類型請參考 `STEP3. HELP`。<br/>
#當網址太長時，可以使用 [PicSee 縮短網址](https://picsee.io/?utm_source=picsee-co&utm_medium=referral&utm_term=home) 來幫助 `命令提示字元(cmd)` 讀取，以避免出錯。<br/><br/>

### I.　PTT Beauty版 下載圖片
在 **PTT Beauty版** 搜尋內容並點選進入後，其網址即為 `-u` ，並將圖片存放於 **./森香澄_img**。
- `-t` PTT
- `-u` https://www.ptt.cc/bbs/Beauty/M.1702040877.A.239.html
- `-p` ./森香澄_img
```
python download_multi_img.py -t ptt -u https://www.ptt.cc/bbs/Beauty/M.1702040877.A.239.html -p ./森香澄_img
```
![森香澄.gif](/森香澄_img/森香澄.gif)
 - 運行完畢後會在 `./森香澄_img` 生成多個 `jpg` 檔。
 - M.1702040877.A.239.html1.jpg
 - ![M.1702040877.A.239.html1.jpg](/森香澄_img/M.1702040877.A.239.html1.jpg)

<br/>

### II.　Unsplash 下載圖片
在 **Unsplash** 以關鍵字 **cat** 搜尋後，其網址即為 `-u` ，並將圖片存放於 **./cat_img**。
- `-t` unsplash
- `-u` https://unsplash.com/s/photos/cat
- `-p` ./cat_img
```
python download_multi_img.py -t unsplash -u https://unsplash.com/s/photos/cat -p ./cat_img
```
 - 運行完畢後會在 `./cat_img` 生成多個 `jpg` 檔。
 - cat12.jpg
 - <img width='426' height='640' src="https://github.com/Junwu0615/Web-Crawler-Download-Img-/blob/2c2de3354369eae1aeaae0b3be9c1b7cf7f24941/cat_img/cat16.jpg"/>


## 參考資源
- [STEAM 教育學習網 | 爬取後同時下載多張圖片](https://steam.oxxostudio.tw/)