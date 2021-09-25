---
title: test
sidebar_label: 1. test
sidebar_position: 200
---

## 문제 
오름차순으로 정렬이 된 두 배열이 주어지면 두 배열을 오름차순으로 합쳐 출력하는 프로그램을 작성하세요.

## 로직

```js
function solution(arr1, arr2){
    var answer = [];
    var n = arr1.length;
    var m = arr2.length;
    var p1 = p2 = 0;
    while(p1 < n && p2 < m){
        if(arr1[p1] <= arr2[p2]) answer.push(arr1[p1++]);
        else answer.push(arr2[p2++]);
    }
    while(p1 < n) answer.push(arr1[p1++]);
    while(p2 < m) answer.push(arr2[p2++]); 
    return answer;
}

var a=[1, 3, 5];
var b=[2, 3, 6, 7, 9];

solution(a, b);
```




