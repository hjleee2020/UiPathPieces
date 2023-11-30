## 1. DateTime 기본형

업무 처리에서 날짜별 처리는 기본이기 때문에 항상 사용되는 변수이다.<br>
본 페이지에서는 DateTime의 기본형을 익히고 UiPath에서 사용되는 예시를 포함하려한다.

물론 해당 사용법을 모두 암기 할필요는 없다! 기본형만 익혀 놓고 쓸때마다 꺼내보자!

`DateTime.Now.ToString()   
DateTime.Now.ToString("MM/dd/yyyy hh:mm:ss")`
--> 11/28/2023 21:19:01

|1|2|
|--|--|
|DateTime.Now.ToString("MM/dd/yyyy")|04-03-2018|
|DateTime.Now.ToString("dddd, dd MMMM yyyy")|화요일, 03 4월 2018|
|DateTime.Now.ToString("dddd, dd MMMM yyyy HH:mm:ss")|화요일, 03 4월 2018 15:55:01|
|DateTime.Now.ToString("MM/dd/yyyy HH:mm")|04-03-2018 15:55|
|DateTime.Now.ToString("MM/dd/yyyy hh:mm tt")|04-03-2018 03:55 오후|
|DateTime.Now.ToString("MM/dd/yyyy H:mm")|04-03-2018 15:55|
|DateTime.Now.ToString("MM/dd/yyyy h:mm tt")|04-03-2018 3:56 오후|
|DateTime.Now.ToString("MM/dd/yyyy HH:mm:ss")|04-03-2018 15:57:07|
|DateTime.Now.ToString("MMMM dd")|4월 03|
|DateTime.Now.ToString("yyyy’-‘MM’-‘dd’T’HH’:’mm’:’ss.fffffffK")|2018’-‘04’-‘03’T’15’:’57’:’31.8282282+09:00|
|DateTime.Now.ToString("ddd, dd MMM yyy HH’:’mm’:’ss ‘GMT’")|화, 03 4 2018 15’:’57’:’53 ‘G4T’|
|DateTime.Now.ToString("yyyy’-‘MM’-‘dd’T’HH’:’mm’:’ss")|2018’-‘04’-‘03’T’15’:’58’:’14|
|DateTime.Now.ToString("HH:mm")|03:58|
|DateTime.Now.ToString("hh:mm tt")|03:58 오후|
|DateTime.Now.ToString("H:mm")|15:58|
|DateTime.Now.ToString("h:mm tt")|3:59 오후|
|DateTime.Now.ToString("HH:mm:ss")|15:59:31|
|DateTime.Now.ToString("yyyy MMMM")|2018 4월|
|DateTime.Now.ToString("yyyyMMdd")|20180403|
|DateTime.Now.ToString("yyyyMMddHHmmss")|20180403160147|


DateTime now = DateTime.Now;

 

DateTime 하루추가 = now.AddDays(1);

 

DateTime 어제날짜 = now.AddDays(-1);

 

 

DateTime 변경날짜 = now.AddYears(1); //1년 추가

 

DateTime 변경날짜 = now.AddMonths(int); //1월 추가

 

DateTime 변경날짜 = now.AddDays(double); // 하루

 

DateTime 변경날짜 = now.AddHours(double);  //시간추가

 

DateTime 변경날짜 = now.AddMinutes(double); //분추가

 

DateTime 변경날짜 = now.AddSeconds(double); //초 추가

 

 

STRING형 -> datetime 형변환

//

string test = "20180828093711";

DateTime = DateTime.ParseExact(test,"yyyyMMddHHmmss",System.Globalization.CultureInfo.InvariantCulture);
