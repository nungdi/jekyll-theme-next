---
title: 20DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**두 정수 사이의 합(level2, javascript)**<br />
adder함수는 정수 a, b를 매개변수로 입력받습니다.<br .<
두 수와 두 수 사이에 있는 모든 정수를 더해서 리턴하도록 함수를 완성하세요. a와 b가 같은 경우는 둘 중 아무 수나 리턴하세요.<br />
예를들어 a가 3, b가 5이면 12를 리턴하면 됩니다.<br /><br />

a, b는 음수나 0, 양수일 수 있으며 둘의 대소 관계도 정해져 있지 않습니다.<br />

{% highlight javascript linenos %}
function adder(a, b){
	var result = 0;

  //함수를 완성하세요
  if (a > b){
    for(var i=b; i<=a; i++){
      result = result + i;
    }
    return result;
	} else if (a < b){
    for(var i=a; i<=b; i++){
      result = result + i;
    }
    return result;
  } else { // a == b
  	return a;
  }
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log( adder(3, 5) )
console.log( adder(5, 5) )
{% endhighlight %}

### 실행결과
12<br />
5

### 출처
[https://programmers.co.kr/learn/challenge_codes/92](https://programmers.co.kr/learn/challenge_codes/92){: target="_blank" }