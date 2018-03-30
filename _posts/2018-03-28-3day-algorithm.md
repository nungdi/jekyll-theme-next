---
title: 3DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**스트링을 숫자로 바꾸기 (level1, javascript)**<br />
strToInt 메소드는 String형 str을 매개변수로 받습니다.<br />
str을 숫자로 변환한 결과를 반환하도록 strToInt를 완성하세요.<br />
예를들어 str이 1234이면 1234를 반환하고, -1234이면 -1234를 반환하면 됩니다.<br />
str은 부호(+,-)와 숫자로만 구성되어 있고, 잘못된 값이 입력되는 경우는 없습니다.<br />

{% highlight javascript linenos %}
function strToInt(str){
  var result = 0;
  //함수를 완성하세요
  result = Number(str);
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(strToInt("-1234"));
{% endhighlight %}

### 실행결과
-1234

### 출처
[https://programmers.co.kr/learn/challenge_codes/110](https://programmers.co.kr/learn/challenge_codes/110){: target="_blank" }
