---
title: 2DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**정수제곱근판별하기 (level1, javascript)**<br />
nextSqaure함수는 정수 n을 매개변수로 입력받습니다.<br />
n이 임의의 정수 x의 제곱이라면 x+1의 제곱을 리턴하고, n이 임의의 정수 x의 제곱이 아니라면 'no'을 리턴하는 함수를 완성하세요.<br />
예를들어 n이 121이라면 이는 정수 11의 제곱이므로 (11+1)의 제곱인 144를 리턴하고, 3이라면 'no'을 리턴하면 됩니다.<br />
{% highlight javascript linenos %}
function nextSqaure(n){
  var result = 0;
  //함수를 완성하세요
  var x = 0;
  while ( x*x < n ){
  	 x++;
  }
  if ( x*x == n ){
    result = Math.pow(x+1, 2);
  } else {
  	 result = 'no';
  }
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log("결과 : " + nextSqaure(121));
console.log("결과 : " + nextSqaure(3));
{% endhighlight %}
### 실행결과
결과 : 144<br />
결과 : no
### 출처
[https://programmers.co.kr/learn/challenge_codes/120](https://programmers.co.kr/learn/challenge_codes/120)
