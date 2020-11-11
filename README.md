## NLP-Notebook

## Installation

```sh
docker-compose up
```

컨테이너를 성공적으로 빌드하고 실행했다면 `localhost:8888`로 jupyter notebook으로 접근할 수 있다.

인증을 받는다.

`notebook` 폴더는 컨테이너와 공유된 폴더로 다른 파일들을 가져와 집어넣으면 jupyter에서 바로 확인할 수 있다. 

`data` 폴더를 만들어 분석할 csv 파일들을 집어넣는다.

현재 가능한 기능은 명사 빈도 추출, 워드클라우드 생성이 있다.