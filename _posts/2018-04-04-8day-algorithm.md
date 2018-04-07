---
title: 8DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**핸드폰번호 가리기 (level1, javascript)**<br />
별이는 헬로월드텔레콤에서 고지서를 보내는 일을 하고 있습니다. <br />
개인정보 보호를 위해 고객들의 전화번호는 맨 뒷자리 4자리를 제외한 나머지를 "\*"으로 바꿔야 합니다. <br />
전화번호를 문자열 s로 입력받는 hide_numbers함수를 완성해 별이를 도와주세요 <br />
예를들어 s가 "01033334444"면 "\*\*\*\*\*\*\*4444"를 리턴하고, "027778888"인 경우는 "\*\*\*\*\*8888"을 리턴하면 됩니다.

{% highlight javascript linenos %}
function hide_numbers(s){
  var result = ""
  
  //함수를 완성해주세요
  var strStart = s.substring(0, s.length - 4);
  var strEnd = s.substr(s.length - 4);
  result = '*'.repeat(strStart.length) + strEnd;
  
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log("결과 : " + hide_numbers('027778888'));
console.log("결과 : " + hide_numbers('01033334444'));
{% endhighlight %}

### 실행결과
결과 : \*\*\*\*\*8888<br />
결과 : \*\*\*\*\*\*\*4444

### 출처
[https://programmers.co.kr/learn/challenge_codes/132](https://programmers.co.kr/learn/challenge_codes/132){: target="_blank" }