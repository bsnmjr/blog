# blog
blog 연습

## 20화 명령줄 지정으로 작업 내용을 바꾸고 싶어 (명령줄 인수)

* 명령줄 인수 (명령어 인자값 혹은 인수) : 명령어를 실행시킬때 스페이스 단위로 입력하는 값들을 말한다.
  - ```cat /data/log/nginx/access.log``` 에서 ```/data/log/nginx/access.log```를 말한다.
  - 명령어 인수1 인수2 인수3 에서 인수1을 쓰고 싶다면 $1을, 인수2를 쓰고 싶다면 $2 를 쓰면 된다.

* 예제코드 (아래 두 개의 쉘스크립트의 공통요소를 찾아 하나의 쉘 스크립트로 수정해보자)

```
#!/bin/bash
DIR=/data/csv
SOURCE="${DIR}/items.csv"
echo "$SOURCE 처리중"
cat $SOURCE
echo "$SOURCE 처리완료"
```
