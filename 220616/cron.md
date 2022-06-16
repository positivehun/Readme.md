# 과제 1
## 현재시간을 1분마다 콘솔에 출력하기
```
0 0/1 * 1/1 * ? *
```

# 과제 2
## 프로그래밍 언어를 사용하여 1분마다 콘솔에 출력하기
```
from time import sleep
from datetime import datetime


while(True):
    print(datetime.today())
    sleep(60)
```

# 과제 3
## 크론표현식 정리

|필드명|값의 허용 범위|허용된 특수 문자|
|:--:|:--:|:--:|
|초(second)|0~59|, - * /|
|분(minute)|0~59|, - * /|
|시(hour)|0~23|, - * /|
|일(day)|1~31|,  - * ? / L W|
|월 (Month)|1 ~ 12 or JAN ~ DEC|, - * /|
|요일 (Week)|0 ~ 6 or SUN ~ SAT|, - * ? / L #|
|연도 (Year)|empty or 1970 ~ 2099|, - * /|
