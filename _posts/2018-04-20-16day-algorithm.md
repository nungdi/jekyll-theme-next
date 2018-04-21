---
title: 16DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**평균구하기(level1, javascript)**<br />
function average(array){
  
  //함수를 완성하세요
  let sum = 0;
  for (let i = 0; i < array.length; i++){
    sum += array[i];
  }
  return sum/array.length;

}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
var testArray = [5,3,4]; 
console.log("평균값 : " + average(testArray));
{% endhighlight %}

### 실행결과
평균값 : 4

### 출처
[https://programmers.co.kr/learn/challenge_codes/126](https://programmers.co.kr/learn/challenge_codes/126){: target="_blank" }