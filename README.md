# hello git

## git 기초 명령어 요약

- clone: 원격 저장소 복사
- add: 스테이지 영역에 작업 파일 추가
- commit: 세이브, 스테이지 영역의 파일들을 가지고 커밋(=세이브)를 만들 수 있다.
- push: 원격 저장소에 커밋을 업로드한다.

## 파일의 내용 되돌리기

- 특정 파일의 내용을 마지막 커밋으로 돌리고 싶다면 해당 파일 선택 후 `코드 뭉치 버리기` 선택

## 브랜치 변경하기

- 브랜치란: 기존 내용을 유지한 채 새로운 내용을 추가하고 싶을 때 사용한다.
- 체크아웃: 특정 브랜치(혹은 커밋)으로 돌아가고 싶을 때 사용.
- 소스트리의 체크아웃: 브랜치 이름을 더블 클릭하는 것만으로 체크아웃 가능


## 병합하기 1

- 헤드 브랜치에 변경사항이 없고
- 병합 대상 브랜치가 헤드로부터 시작된 경우
- 아주 쉽게 병합 가능 = Fast-forward


## 병합하기 2

- 헤드 브랜치에 추가적인 커밋이 생기는 경우
- 진짜 병합이 필요해진다.
- 충돌이 안 나면 좋은데, 충돌이 나도 겁내지 말자. 


## 충돌 해결하기

- 제일 중요한 점: 겁내지 말아요!
- 같은 파일을 병합 대상 두 커밋에서 동시 수정했을 경우 충돌이 날 확률이 높다!
- 에디터 사용, 혹은 SoureTree를 사용해서 충돌 해결 가능하다.


## 커밋 되돌리기

### reset 사용하기

- 장점: 쉬움.
- 단점1: 커밋이 날아간다. 
- 단점2: 강제 푸시가 필요하다.


### branch 만들어서 되돌리기

- reset과는 달리 내용이 사라지지 않는다.
- 장점: 쉽다.
- 단점: 트리가 지저분해진다.

### revert

- 역시 커밋은 없어지지 않는다.
- 장점: 가장 정석적이다. 커밋은 남고 작업 이력만 이전것으로 보여준다.
- 단점: 충돌이 날 수 있다. 
