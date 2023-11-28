## 1. ForEach 를 사용!
![foreach](https://github.com/hjleee2020/UiPathPieces/assets/152233743/a5afba47-cc05-418a-8e63-8a87958cc4f3)

Assign 하여 리스트 타입 변수에 "1,2,3,4,5,6,7,8,9"의 변수를 넣고 foreach 를 사용하여 출력하였다.<br>
여기서 주목할 부분은 ForEach에 currentitem에 aGugu 변수의 값이 순서대로 입력된다는 것이고,<br>
0번부터 8번째까지 총 9번 foreach문이 작동하는 점이다.

(:smile:보너스) 속성 부분에 TypeArgument 는 currentitem에 입력되는 변수 형태를 지정하는 것!

<br>

## 2. 구구단을 만들자!

![gugudan](https://github.com/hjleee2020/UiPathPieces/assets/152233743/a2224b92-5a33-4f7e-97d9-234688abe277)

foreach 안에 foreach를 작성하여 구구단을 만들었다!
