---
title: 10DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**문자열 내 p와 y의 개수 (level1, javascript)**<br />
numPY함수는 대문자와 소문자가 섞여있는 문자열 s를 매개변수로 입력받습니다.<br />
s에 'p'의 개수와 'y'의 개수를 비교해 같으면 True, 다르면 False를 리턴하도록 함수를 완성하세요.<br />
'p', 'y' 모두 하나도 없는 경우는 항상 True를 리턴합니다.<br />
예를들어 s가 pPoooyY면 True를 리턴하고 Pyy라면 False를 리턴합니다.

{% highlight javascript linenos %}
function numPY(s){
  var result = false;
  
  //함수를 완성하세요
  var p = s.match(/p/gi).length;
  var y = s.match(/y/gi).length;
  
  if ( (p == y) || (p, y == 0) ){
  	result = true;
  }
  
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log( numPY("pPoooyY") )
console.log( numPY("Pyy") )
{% endhighlight %}

### 실행결과
true<br />
false

### 출처
[https://programmers.co.kr/learn/challenge_codes/96](https://programmers.co.kr/learn/challenge_codes/96){: target="_blank" }
