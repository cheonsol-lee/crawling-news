# rawling-news
국내/외 뉴스 크롤링

#### *Made by cheonsol lee - Updated(2020.08.12)* ####

----------
### 1. 목적
* 국내 뉴스 : 네이버
* 국외 뉴스 : CNN(미국), BBC(영국), CTV(캐나다)
* 위키 백과 : 국내/외

국내/외 뉴스와 위키백과 사이트를 크롤링하여 기사제목은 파일명으로, 기사내용은 파일내용으로 하는 텍스트 파일을 제작한다.


----------
### 2. 특징
* 정적크롤링을 이용했기에 beautifulSoup만으로 구현이 가능하였다.
* 디렉토리 경로가 없을 경우, 미리 생성 후에 파일을 생성한다.


----------
### 3. 설치할 것

import requests
from bs4 import BeautifulSoup
import re
import os


----------
### 4. 실행방법
* language, item, news를 입력하면 xx/xx/xx.txt 형태의 파일이 생성된다.
* url에 해당 기사의 url을 입력한다.
* Run의 crawling()함수를 실행하면 설정한 경로에 '기사제목.txt'형태의 파일이 생성된다.
  * ex) 기사제목.txt
