## 리눅스 프로그래밍 시작하기

### gcc를 이용한 빌드
참고 링크
1. https://digiconfactory.tistory.com/entry/%EC%9C%88%EB%8F%84%EC%9A%B010-%EC%9A%B0%EB%B6%84%ED%88%AC-%EB%A6%AC%EB%88%85%EC%8A%A4-WSL2-%EC%84%A4%EC%B9%98
2. https://ko.wikihow.com/%EB%A6%AC%EB%88%85%EC%8A%A4%EC%9D%98-%ED%84%B0%EB%AF%B8%EB%84%90%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%B4%EC%84%9C-%ED%85%8D%EC%8A%A4%ED%8A%B8-%ED%8C%8C%EC%9D%BC%EC%9D%84-%EC%83%9D%EC%84%B1%ED%95%98%EA%B3%A0-%ED%8E%B8%EC%A7%91%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95
<br/>
참고 서적
1. 모두를 위한 리눅스 프로그래밍(아오키 미네로)

### 기본 순서
1. Ubuntu 열기
2. mkdir 및 cd
3. vi 파일명.c
4. vim으로 파일 작성
5. esc 누르고 : **w(문서저장)**, **:q(문서종료)**, **:i(파일수정)**
6. 소스코드 빌드: **gcc 파일명.c**
7. a.out 생성 확인: **ls**
8. 생성된 파일 실행: **./a.out** 

<br/><br/>
## gcc를 이용한 빌드(2)
#### 실행 파일 이름 변경
1. (rm a.out) -> 이전에 실행된 a.out은 미리 지워둔다
2. gcc -o 원하는실행파일명 실행파일.c
- gcc -o hello hello.c
3. ./실행파일명
- ./hello

<br/>
### 버그와 디버깅
작성한 프로그램에 문제가 있는 경우
실행파일 입력 시 Segmentation fault 등이 출력됨
이러한 버그를 없애기 위한 조사 및 수정 작업이 디버그(debug)

#### 디버그를 위한 가장 대중적인 방법: 
1. **printf 신공**: 값 출력
2. **디버거 이용**: 리눅스 개발 시에는 gbd가 많이 사용됨

#### 
