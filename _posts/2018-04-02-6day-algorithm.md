---
title: 6DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**피보나치 수 (level1, javascript)**<br />
피보나치 수는 F(0) = 0, F(1) = 1일 때, 2 이상의 n에 대하여 F(n) = F(n-1) + F(n-2) 가 적용되는 점화식입니다. <br />
2 이상의 n이 입력되었을 때, fibonacci 함수를 제작하여 n번째 피보나치 수를 반환해 주세요. <br />
예를 들어 n = 3이라면 2를 반환해주면 됩니다.<br /><br />

처음에 재귀함수로 풀었으나 ...

{% highlight javascript linenos %}
function fibonacci(num) {
	if (num < 2){
    return num;
  } else {
    return fibonacci(num-1) + fibonacci(num-2);
  }
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(fibonacci(3))
{% endhighlight %}

### 실행결과
실행시간이 5초를 초과하여 실행이 중단되었습니다. T^T

<br />
배열을 선언하고 배열에 값을 추가하는 방식 으로풀이 ...

{% highlight javascript linenos %}
function fibonacci(num) {
  var answer = 0,
      cache = [0,1];

  if ( num < 2 ){
    answer = num;
  } else {
    for (var i = 2; i <= num; i++ ) {
      cache.push(cache[i-1] + cache[i-2]); 
      answer = cache[i];
    } 
  }

  return answer;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(fibonacci(3));
{% endhighlight %}

### 실행결과
2

### 출처
[https://programmers.co.kr/learn/challenge_codes/6](https://programmers.co.kr/learn/challenge_codes/6){: target="_blank" }
