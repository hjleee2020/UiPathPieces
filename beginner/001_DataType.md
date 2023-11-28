## 1. 기본 변수 형태 4분류
1. 문자형
2. 정수형
3. 실수형
4. 논리형
<br><br>
## 2. 기본 변수 형태 8개!
|분류|설명|예시|
|------|---|---|
|문자형|문자 사용|char|
|정수형|0을 포함한 정수|byte, short, int, long|
|실수형|실수|float, double|
|논리형|참, 거짓 같은 논리 값|boolean|

<br><br>
## 3. UiPath에 자주 사용되는 변수
|DataType|설명|예시|
|------|---|---|
|Boolean|논리형 변수예(=true) 아니오(=false)를 정의한다.|ture, false|
|Int32|0을 포함한 정수|byte, short, int, long|
|String|문자열 형식을 의미|float, double|
|Object|모든 데이터 형식을 받을 수 있는 변수.<br>다양한 용도로 정말 많이 사용된다.|중요!|
|DataTable|데이터를 저장하는 테이블 <br>테이블 row column에 대한 이해가 필요!|중요!|
|Array of [T]|배열 타입의 변수, <br>다양한 형식 데이터를 사용하여 다양한 형식의 배열을 생성 한다.|{1,2,3,4}  {가,나,다,라}|

<br>

## 4. 캐스팅!(명시적)
데이터 처리간 많은 자료형이 사용된다. 특히 string int 간 명시적 캐스팅을 사용하는 경우가 정말 많다!

<br>

## 5. 변수 명명 규칙

정해진 규칙은 아니나 일반적으로 사용된다. 업무 환경에 따라 바뀔 수 있으니 참고만 하자

|접두어|의미|
|------|---|
|a|array 배열|
|b|boolean 형 변수|
|By|BYTE 형 변수|
|d|DateTime 형 변수|
|dbl|Double 형 변수(소수점포함)|
|f|Float 형 변수 (소수점 포함)|
|g_|Global 변수(전역 변수)|
|h|Handle 형 변수|
|i|정수 형 변수|
|l|long 형 변수|
|s|String 문자열|
|dt|DataTable 형 변수|


<br>

## (보너스) 캐스팅 및 형식 변환(C# 프로그래밍 가이드)
출처:https://learn.microsoft.com/ko-kr/dotnet/csharp/programming-guide/types/casting-and-type-conversions
