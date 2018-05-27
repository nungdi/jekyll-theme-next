---
title: 24DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**야근 지수(level2, javascript)**<br />
n회사원 Demi는 가끔은 야근을 하는데요, 야근을 하면 야근 피로도가 쌓입니다. 야근 피로도는 야근을 시작한 시점에서 남은 일의 작업량을 제곱하여 더한 값입니다. Demi는 N시간 동안 야근 피로도를 최소화하도록 일할 겁니다.Demi가 1시간 동안 작업량 1만큼을 처리할 수 있다고 할 때, 퇴근까지 남은 N 시간과 각 일에 대한 작업량 works에 대해 야근 피로도를 최소화한 값을 리턴하는 함수 solution을 완성해주세요.

*제한 사항*
works는 길이 1 이상, 20,000 이하인 배열입니다.
works의 원소는 50000 이하인 자연수입니다.
n은 1,000,000 이하인 자연수입니다.
*입출력 예*
<table>
  <colgroup>
    <col width="70px" />
    <col width="27px" />
    <col width="60px" />
  </colgroup>
  <tr>
    <th>works</th>
    <th>n</th>
    <th>result</th>
  </tr>
  <tr>
    <td>[4, 3, 3]</td>
    <td>4</td>
    <td>12</td>
  </tr>
  <tr>
    <td>[2, 1, 2]</td>
    <td>1</td>
    <td>6</td>
  </tr>
  <tr>
    <td>[1,1]</td>
    <td>3</td>
    <td>0</td>
  </tr>
</table>


{% highlight javascript linenos %}
function solution(n, works) {
  var answer = 0;
  var sum = works.reduce((a, b) => a + b, 0);
  if (n < sum) {
    for (var i = 0; i < n; i++) {
      var idx = works.indexOf(Math.max.apply(null, works));
      works[idx] -= 1;
    }
    answer = works.reduce((answer, x) => answer + Math.pow(x, 2), 0);
  }
  return answer;
}
{% endhighlight %}

### 실행결과
테스트를 통과하였습니다.

### 출처
[https://programmers.co.kr/learn/courses/30/lessons/12927?language=javascript](https://programmers.co.kr/learn/courses/30/lessons/12927?language=javascript){: target="_blank" }