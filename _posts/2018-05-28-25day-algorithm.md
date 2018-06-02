---
title: 25DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**숫자의 표현(level2, javascript)**<br />
Finn은 요즘 수학공부에 빠져 있습니다. 수학 공부를 하던 Finn은 자연수 n을 연속한 자연수들로 표현 하는 방법이 여러개라는 사실을 알게 되었습니다. 예를들어 15는 다음과 같이 4가지로 표현 할 수 있습니다.

<ul>
<li>1 + 2 + 3 + 4 + 5 = 15</li>
<li>4 + 5 + 6 = 15</li>
<li>7 + 8 = 15</li>
<li>15 = 15</li>
</ul>

자연수 n이 매개변수로 주어질 때, 연속된 자연수들로 n을 표현하는 방법의 수를 return하는 solution를 완성해주세요.

*제한 사항*
n은 10,000 이하의 자연수 입니다.

*입출력 예*
<table>
  <colgroup>
    <col width="27px" />
    <col width="60px" />
  </colgroup>
  <tr>
    <th>n</th>
    <th>result</th>
  </tr>
  <tr>
    <td>15</td>
    <td>4</td>
  </tr>
</table>


{% highlight javascript linenos %}
function solution(n) {
    var answer = 0;
    var sum = 0, j;
    for ( var i = 1; i <= n; i++ ) { 
        sum = 0, j = i;
        while ( sum <= n ) { 
            sum += j; 
            if ( sum === n ) answer++;
            j++ 
        }
    }
    return answer;
}
{% endhighlight %}

### 실행결과
테스트를 통과하였습니다.

### 출처
[https://programmers.co.kr/learn/courses/30/lessons/12924?language=javascript](https://programmers.co.kr/learn/courses/30/lessons/12924?language=javascript){: target="_blank" }