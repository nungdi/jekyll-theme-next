---
title: 12DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**수박수박수박수박수박수?**<br />
water_melon함수는 정수 n을 매개변수로 입력받습니다.<br />
길이가 n이고, 수박수박수...와 같은 패턴을 유지하는 문자열을 리턴하도록 함수를 완성하세요.<br /><br />

예를들어 n이 4이면 '수박수박'을 리턴하고 3이라면 '수박수'를 리턴하면 됩니다.

{% highlight javascript linenos %}
function waterMelon(n){
  var result = ""
  
  //함수를 완성하세요
  for ( var i = 1; i <= n; i ++) {
  	if (i%2 == 1) {
  		result += '수'
  	} else {
  		result += '박'
  	}
  }
  
  return result;
}

// 실행을 위한 테스트코드입니다.
console.log("n이 3인 경우: "+ waterMelon(3))
console.log("n이 4인 경우: "+ waterMelon(4))
{% endhighlight %}

### 실행결과
n이 3인 경우: 수박수<br />
n이 4인 경우: 수박수박

### 출처
[https://programmers.co.kr/learn/challenge_codes/107](https://programmers.co.kr/learn/challenge_codes/107){: target="_blank" }