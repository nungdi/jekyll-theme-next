---
title: 26DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**제일 작은 수 제거하기(level1, javascript)**<br />
정수를 저장한 배열, arr 에서 가장 작은 수를 제거한 배열을 리턴하는 함수, solution을 완성해주세요. 단, 리턴하려는 배열이 빈 배열인 경우엔 배열에 -1을 채워 리턴하세요. 예를들어 arr이 [4,3,2,1]인 경우는 [4,3,2]를 리턴 하고, [10]면 [-1]을 리턴 합니다.

*제한 사항*
<ul>
  <li>arr은 길이 1 이상인 배열입니다.</li>
  <li>인덱스 i, j에 대해 i ≠ j이면 arr[i] ≠ arr[j] 입니다.</li>
</ul>

*입출력 예*
<table>
  <colgroup>
    <col width="27px" />
    <col width="60px" />
  </colgroup>
  <tr>
    <th>arr</th>
    <th>result</th>
  </tr>
  <tr>
    <td>[4,3,2,1]</td>
    <td>[4,3,2]</td>
  </tr>
  <tr>
    <td>[10]</td>
    <td>[-1]</td>
  </tr>
</table>


{% highlight javascript linenos %}
function solution(arr) {
    var answer = [];
    if ( arr.length > 1 ){
        var $min = Math.min.apply(null, arr);
        var idx = arr.indexOf($min);
        answer = arr.splice(idx, 1);
    } else {
        answer = [-1];
    }
    return answer;
}
{% endhighlight %}

### 실행결과
테스트를 통과하였습니다.

### 출처
[https://programmers.co.kr/learn/courses/30/lessons/12935?language=javascript](https://programmers.co.kr/learn/courses/30/lessons/12935?language=javascript){: target="_blank" }