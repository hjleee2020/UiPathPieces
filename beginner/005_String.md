String 문자열 다루기!

## 1. 스트링 내부에 존재하는 메소드!

### Length
문자열 길이 반환하였습니다.

### Split
```
string original = "안녕하세요 화이팅입니다!";
string[] split_data = original.Split(' ');
```
=> '안녕하세요'와 '화이팅입니다!'가 split_data에 저장됩니다.<br>
Uipath에서는 주로 original.Split(' ')[1] 처럼 문자열에서 해당 문자열을 선택하는 방식으로 많이 사용했다.<br>
특히, 메일에서 특정 메시지를 추출하는 것에 많이 사용했다.

### Trim
문자열의 양쪽 공백을 잘라냄!<br>
html을 selecter를 통해 가져오는 uipath 구조상 텍스트 양쪽에 공백이나 줄바꿈이 포함되어 있는 경우가 잦다!<br>
인식이 안된다면 꼭한번 공백을 확인해보자! <br>
(사례) 콤보박스 리스트를 가져오는 과정에서 발생


## 2. 스트링을 다루는 메소드!

### Replace
문자열 치환하는 메소드이다!
```
str = "ABCDEFG"
str2 = str.Replace("CD","AA")
```
=> str2 는 ABAAEFG값을 갖는다!

### Substring
문자열 자르기!!
```string str = "123456789"
str.Substring(0, 4) = 1234
```


### 3. 정규표현식
https://learn.microsoft.com/ko-kr/dotnet/standard/base-types/regular-expressions
