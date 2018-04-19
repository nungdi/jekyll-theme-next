---
title: 15DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**다음 큰 숫자(level3, javascript)**<br />
어떤 수 N(1≤N≤1,000,000) 이 주어졌을 때, N의 다음 큰 숫자는 다음과 같습니다.
<ul>
	<li>N의 *다음 큰 숫자*는 N을 2진수로 바꾸었을 때의 1의 개수와 같은 개수로 이루어진 수입니다.</li>
	<li>1번째 조건을 만족하는 숫자들 중 N보다 큰 수 중에서 가장 작은 숫자를 찾아야 합니다.</li>
</ul>
예를 들어, 78을 2진수로 바꾸면 1001110 이며, 78의 *다음 큰 숫자*는 83으로 2진수는 1010011 입니다.<br />
N이 주어질 때, N의 *다음 큰 숫자*를 찾는 nextBigNumber 함수를 완성하세요.

{% highlight javascript linenos %}
function nextBigNumber(n){
  
  let _two = n.toString(2).split('').filter(num => 1 === parseInt(num, 10)).length;
  
  while(true){
    n += 1
    if(n.toString(2).split('').filter(num => 1 === parseInt(num, 10)).length === _two){
      break;
    }
  }
  return n;
        
}

//아래 코드는 테스트를 위한 코드입니다.
console.log(nextBigNumber(78));
{% endhighlight %}

### 실행결과
83

### 출처
[https://programmers.co.kr/learn/challenge_codes/174](https://programmers.co.kr/learn/challenge_codes/174){: target="_blank" }