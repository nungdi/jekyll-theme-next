---
title: 14DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**괄호 확인하기(level2, javascript)**<br />
is_pair함수는 문자열 s를 매개변수로 입력받습니다.<br />
s에 괄호가 알맞게 짝지어져 있으면 True를 아니면 False를 리턴하는 함수를 완성하세요.<br />
예를들어 s가 (hello)()면 True이고, )(이면 False입니다.<br />
s가 빈 문자열("")인 경우는 없습니다.

{% highlight javascript linenos %}
function is_pair(s){
  var result = true;
  
  // 함수를 완성하세요
  var txt = s.match(/(\(|\))/g);
  if (txt[0] == '(' && (txt.length % 2) == 0){
  	result = true;
  } else {
  	result = false;
  }
  
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log( is_pair("(hello)()") )
console.log( is_pair(")(") )
{% endhighlight %}

### 실행결과
true<br />
false

### 출처
[https://programmers.co.kr/learn/challenge_codes/87](https://programmers.co.kr/learn/challenge_codes/87){: target="_blank" }