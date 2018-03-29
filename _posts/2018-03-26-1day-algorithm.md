---
title: 1DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm, study, javascript
---

알고리즘 스터디 첫번째

문제)
evenOrOdd 메소드는 int형 num을 매개변수로 받습니다.
num이 짝수일 경우 Even을 반환하고 홀수인 경우 Odd를 반환하도록 evenOrOdd에 코드를 작성해 보세요.
num은 0이상의 정수이며, num이 음수인 경우는 없습니다.

# Highlight block

{% highlight javascript %}
function evenOrOdd(num) {
  var result = ''
  // 함수를 완성하세요
  if ( num % 2 == 0 ){
    return 'Even';
  } else {
    return 'Odd';
  }
  return result;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log("결과 : " + evenOrOdd(2));
console.log("결과 : " + evenOrOdd(3));
{% endhighlight %}

