---
title: 21DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

### 문제
**이상한 문자만들기(level2, javascript)**<br />
toWeirdCase함수는 문자열 s를 매개변수로 입력받습니다.<br />
문자열 s에 각 단어의 짝수번째 인덱스 문자는 대문자로, 홀수번째 인덱스 문자는 소문자로 바꾼 문자열을 리턴하도록 함수를 완성하세요.<br />
예를 들어 s가 try hello world라면 첫 번째 단어는 TrY, 두 번째 단어는 HeLlO, 세 번째 단어는 WoRlD로 바꿔 TrY HeLlO WoRlD를 리턴하면 됩니다.<br /><br />
**주의** 문자열 전체의 짝/홀수 인덱스가 아니라, 단어(공백을 기준)별로 짝/홀수 인덱스를 판단합니다.

{% highlight javascript linenos %}
function toWeirdCase(s){
  var result = [];
  var str = s.split(' ');
  for(var i = 0; i < str.length; i++){
    var el = [];
    for(var j = 0; j<str[i].split('').length; j++){
      if ( j%2 != 0 ){
        el.push(str[i].split('')[j].toLowerCase());
      } else {
        el.push(str[i].split('')[j].toUpperCase());
      }
    }
    result.push(el.join(''));
  }
  return result.join(' ');
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log("결과 : " + toWeirdCase("try hello world"));

{% endhighlight %}

### 실행결과
결과 : TrY HeLlO WoRlD

### 출처
[https://programmers.co.kr/learn/challenge_codes/114](https://programmers.co.kr/learn/challenge_codes/114){: target="_blank" }