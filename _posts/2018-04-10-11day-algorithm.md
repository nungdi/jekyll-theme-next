---
title: 11DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**약수의 합 (level1, javascript)**<br />
어떤 수를 입력받아 그 수의 약수를 모두 더한 수 sumDivisor 함수를 완성해 보세요.<br />
예를 들어 12가 입력된다면 12의 약수는 [1, 2, 3, 4, 6, 12]가 되고, 총 합은 28이 되므로 28을 반환해 주면 됩니다.

{% highlight javascript linenos %}
function sumDivisor(num) {
	var answer = 0;
  
  for ( var i = 1; i <= num; i++ ){
  	if ( num%i == 0 ){
    	answer += i;
    }
  }

	return answer;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(sumDivisor(12));
{% endhighlight %}

### 실행결과
28

### 출처
[https://programmers.co.kr/learn/challenge_codes/3](https://programmers.co.kr/learn/challenge_codes/3){: target="_blank" }