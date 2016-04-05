# Python 환경 세팅
Python 및 데이터 분석에 필요한 환경 설정


## 1. 설치

1-1. python 3
  - python 2.7 vs python 3
  - 차이? python 3은 유니코드 (한글..), print
  - python2
    * ** coding : UTF-8 **
    * print "문자열" vs print()

1-2. 환경변수
  - C:\Python35;C:\Python35\Scripts;C:\Python35\Lib\site-packages;

2. ez_setup : easy_install (패스)
```
# easy_install [모듈명]
```

3. pip : 라이브러리 설치.. (패스)
```
# pip install [모듈명]
```
  - proxy 설정 필요
  - 사내에서 정상 설치안되므로 -->  whl 수동설치.
  - **proxy 설정 공유 (다음시간에..)**

4. anaconda
  - numpy, scipy, ipython, pandas...
  - [anaconda 다운로드](https://www.continuum.io/downloads)

4-1. 환경변수
  - C:\Anaconda3\Scripts
  - [github pyrian](https://github.com/pyrian/data-analysis-killer)

  ```
  # git clone https://github.com/pyrian/data-analysis-killer

  <!-- git proxy 설정 -->
  # git config --global http.proxy [ip]:[port]
  # git config --global https.proxy [ip]:[port]
  ```

## [참조]
window에서 설치 시는 path 설정 필요


## 2. ipython notebook vs idle
 - 개발환경 세팅
 - ipython notebook

## 3. OS X
 - .bash_profile : python 경로 바꾸고. anaconda --> python3
 - 가상환경 제공, virtualenv , virtualwrapper

## 4. ipython auto save time setting
```
$([IPython.events]).on("notebook_loaded.Notebook", function () {
  IPython.notebook.set_autosave_interval(0);
});
```
$(ipython locate profile)/static/custom/custom.js.
The value is in milliseconds.

## 5. Jupyter 설치 (ipytnon 에서 버전업 ??)
1. https://www.continuum.io/downloads anaconda 다운로드 후 인스톨

2. Proxy 설정
  - c:\Users\사용자명\ .condarc 파일 생성
  ```
    proxy_servers:
        http: http://ip:port
        https: http://ip:port
    ssl_verify: False
  ```

3. Commnad 라인에 conda install jupyter 입력

4. jupyter notebook 실행
