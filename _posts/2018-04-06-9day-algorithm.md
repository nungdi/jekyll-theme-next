---
title: 9DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**2016년 (level2, javascript)**<br />
2016년 1월 1일은 금요일입니다. <br />
2016년 A월 B일은 무슨 요일일까요? <br />
두 수 A,B를 입력받아 A월 B일이 무슨 요일인지 출력하는 getDayName 함수를 완성하세요. <br />
요일의 이름은 일요일부터 토요일까지 각각 \'SUN,MON,TUE,WED,THU,FRI,SAT\'를 출력해주면 됩니다. <br />
예를 들어 A=5, B=24가 입력된다면 5월 24일은 화요일이므로 TUE를 반환하면 됩니다.

{% highlight javascript linenos %}
function getDayName(a,b){
	let answer = "";
  let date = new Date(`2016, ${a}, ${b}`);
  answer = date.toString().substring(0, 3).toUpperCase();
  
  return answer;
  //console.log(date);
}

//아래 코드는 테스트를 위한 코드입니다.
console.log(getDayName(5,24));
{% endhighlight %}

### 실행결과
TUE

### 출처
[https://programmers.co.kr/learn/challenge_codes/178](https://programmers.co.kr/learn/challenge_codes/178){: target="_blank" }
