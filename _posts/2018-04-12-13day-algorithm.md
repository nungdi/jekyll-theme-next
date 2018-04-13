---
title: 13DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**행렬의 덧셈(level1, javascript)**<br />
행렬의 덧셈은 행과 열의 크기가 같은 두 행렬의 같은 행, 같은 열의 값을 서로 더한 결과가 됩니다. <br />
2개의 행렬을 입력받는 sumMatrix 함수를 완성하여 행렬 덧셈의 결과를 반환해 주세요.<br /><br />

예를 들어 2x2 행렬인 A = ((1, 2), (2, 3)), B = ((3, 4), (5, 6)) 가 주어지면, 같은 2x2 행렬인 ((4, 6), (7, 9))를 반환하면 됩니다.(어떠한 행렬에도 대응하는 함수를 완성해주세요.)<br /><br />

예를들어 n이 4이면 '수박수박'을 리턴하고 3이라면 '수박수'를 리턴하면 됩니다.

{% highlight javascript linenos %}
function sumMatrix(A,B){
  var answer = Array();
  
  for(var i = 0; i < A.length; i++){
    answer[i] = [];
    for(var j = 0; j < A[i].length; j++){
      answer[i][j] = A[i][j] + B[i][j];       
    }
  }
  
  return answer;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(sumMatrix([[1,2], [2,3]], [[3,4],[5,6]])) 
{% endhighlight %}

### 실행결과
[ [ 4, 6 ], [ 7, 9 ] ]

### 출처
[https://programmers.co.kr/learn/challenge_codes/9](https://programmers.co.kr/learn/challenge_codes/9){: target="_blank" }