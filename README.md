# JAVA_RMS

Study JAVA for RMS in Bistelligence



#### 자동완성 세팅

Window -> Preferences -> Java -> Editor -> Content Assist
하단에 Auto activation에 Auto activation triggers for Java에
점(.)만 찍혀있는데 .abcdefghijklmnopqrstuvwxyz 로 바꿔주기

#### eclipse 단축키

1. ctrl + shift + L : 단축키 전체 목록보기
2. ctrl + '+'/'-' : 폰트 크기 조절
3. ctrl + D : 한 줄 삭제
4. ctrl + alt + down 행단위 복사
5. alt + shift + A : 멀티컬럼 편집
6. alt + ↑/↓ : 행단위 이동
7. ctrl + i : 자동 들여쓰기
8. ctrl + space : 자동완성
   1. ex) sysout 입력 후 ctrl + space -> System.out.priltln("") 자동입력됨
   2. sysout과 같이 커멘드는 편집 가능
      Window -> Preferences -> Java -> Editor -> Templates 에서 편집하면 됨
      Edit을 누르면 yes / no 가 뜨는데 no 누를것!
      (yes는 기존 단축키 유지한 상태에서 추가하기 / no는 변경하기)



#### 변수

하나의 값을 저장할 수 있는 메모리 공간(RAM)

1. 변수의 선언 이유
   - 값(data)을 저장할 공간을 마련하기 위해
2. 변수의 선언 방법
   - 변수의  선언 방법: **변수타입** **변수이름;**
   - **int** **age;**    // 정수(int)타입의 변수 age를 선언
3. 변수에 값 저장하기 ('=' 연산자는 등호(같다)가 아니라 대입)
   - **int age;**
     **age = 25;**
   - **int x = 0, y = 5;**   // 이런 식으로도 가능



#### 변수의 타입

문자 - char

숫자

1. 정수 - byte, short, int, long
2. 실수 - float, double

논리 - boolean(true, false)



#### 상수

한 번만 값을 저장 가능한 변수

선언 방식은 변수와 동일하나 앞에 'final' 추가
final int MAX = 100; // MAX는 상수, 이후 MAX = 200; 코드치면 에러남

#### 리터럴

그 자체로 값을 의미하는 것
1, 2, 3, 'a', 'b', 'c', '가', 등등

