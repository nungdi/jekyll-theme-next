---
title: 5DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**문자열 다루기 기본 (level1, javascript)**<br />
alpha_string46함수는 문자열 s를 매개변수로 입력받습니다.<br />
s의 길이가 4혹은 6이고, 숫자로만 구성되있는지 확인해주는 함수를 완성하세요.<br />
예를들어 s가 a234이면 False를 리턴하고 1234라면 True를 리턴하면 됩니다<br />

{% highlight javascript linenos %}
function alpha_string46(s){
  var result = true
  // 함수를 완성하세요
	 if ( (s.length == 4 || s.length == 6) && /^[0-9]+$/.test(s) ){
    result = true;
  } else {
  	 result = false;
  }
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log( alpha_string46("1234") );
console.log( alpha_string46("a234") );
{% endhighlight %}

### 실행결과
true<br />
false

### 출처
[https://programmers.co.kr/learn/challenge_codes/99](https://programmers.co.kr/learn/challenge_codes/99){: target="_blank" }
