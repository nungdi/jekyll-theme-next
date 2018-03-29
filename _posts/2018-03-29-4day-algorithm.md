---
title: 4DAY, ALGORITHM
categories:
 - ALGORITHM
tags: algorithm study javascript
---

알고리즘 스터디 네번째

문제)
최대공약수와 최소공배수 (level1, javascript)
두 수를 입력받아 두 수의 최대공약수와 최소공배수를 반환해주는 gcdlcm 함수를 완성해 보세요. 
배열의 맨 앞에 최대공약수, 그 다음 최소공배수를 넣어 반환하면 됩니다. 
예를 들어 gcdlcm(3,12) 가 입력되면, [3, 12]를 반환해주면 됩니다.

{% highlight javascript linenos %}
function gcdlcm(a, b) {
    var answer = [];
  	var mathMin = Math.min(a, b);
  	var _max = 1;
  	var range = mathMin;
  	for(var i=1; i<=range; i++){
    	if( a % i == 0 && b % i == 0){
        _max = i;
      }
    }
 		var _min = a * b / _max;
  	answer[0] = _max;
  	answer[1] = _min;
  
    return answer;
}

// 아래는 테스트로 출력해 보기 위한 코드입니다.
console.log(gcdlcm(3,12));
{% endhighlight %}

실행결과 : [ 3, 12 ]
