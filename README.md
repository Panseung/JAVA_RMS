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



#### 기본형과 참조형

1. **기본형**: 실제 값을 저장

   1. boolean
   2. char
   3. byte
   4. short
   5. int
   6. long
   7. float
   8. double

2. **참조형**: 메모리 주소를 저장(4byte or 8byte)

   기본형을 제외한 나머지 (String, System 등)

3. 기본형의 크기

   | 종류 / 크기(byte) | 1       | 2     | 3     | 4      |
   | ----------------- | ------- | ----- | ----- | ------ |
   | 논리형            | boolean |       |       |        |
   | 문자형            |         | char  |       |        |
   | 정수형            | byte    | short | int   | long   |
   | 실수형            |         |       | float | double |

   1bit = 2진수 1자리
   1byte = 8bit

   

#### printf()의 지시자

1. %b : boolean
2. %d : 10진
3. %o : 8진
4. %x : 16진
5. %f : 부동소수점
6. %e : 지수
7. %c : 문자
8. %s : 문자열

```java
System.out.printf("age:%d year:%d\n", 14, 2017)
```

printf()는 줄바꿈을 하지 않기 때문에 줄바꿈이 필요하면 끝에 %n or \n을 붙여줘야함
(\n은 OS마다 줄바꿈이 될 수도 있고 안될수도 있기 때문에 OS와 관계없이
줄바꿈이 가능한 %n 추천)

```java
System.out.printf("[%5d]%n", 10); 	//[   10]
System.out.printf("[%-5d]%n", 10);	//[10   ]
System.out.printf("[%05d]%n", 10);	//[00010]
```



#### Scanner

1. 화면으로부터 데이터를 입력받는 기능을 제공하는 클래스

2. 사용 순서

   1. import문 추가
      ```java
      import java.util.*;
      ```

   2. Scanner객체의 생성
      ```java
      Scanner scanner = new Scanner(System.in);
      ```

   3. Scanner객체를 사용
      ```java
      int num = scanner.nextInt();  // 화면에서 입력받은 정수를 num에 저장
      String input = scanner.nextLine();  // 화면에서 입력받은 내용을 input에 저장
      int num = Integer.parseInt(input); // 문자열(input)을 숫자로 변환
      ```

      
