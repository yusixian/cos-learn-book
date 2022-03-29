# 2022春网易雷火前端暑期实习笔试(AK)

* 选择7道 21分
* 不定项5道 30分
* 填空2道 多少分来着
* 问答2道 不记得了
* 编程题3道 easy easy middle水平，核心代码模式，总码量不到40行- -

20分钟写完编程就交卷出来玩了，啧

## 问答-2 get函数实现

笔试完，用copilot补全出来了 乐

```js
let obj = {a:[{b: {c: 1}}]}
// console.log(obj.a[0].b.c)
function get(obj, str) {
    str = str.split('.')
    let len = str.length
    for(let i = 0; i < len; ++i) {
        if(str[i] && str[i].indexOf('[') != -1) {
            let index = str[i].match(/\[(\d+)\]/)[1]
            let name = str[i].split('[')[0]
            if(name in obj) {
                obj = obj[name][index]
            } else {
                return undefined
            }
        } else if(str[i] in obj && obj[str[i]]) {
            obj = obj[str[i]]
        } else {
            return undefined
        }
    }
    return obj
}
console.log(get(obj, 'a[0].b.c'))
console.log(get(obj, 'a[0].b.s'))
console.log(get(obj, 'a.s.q'))
```

## 编程题-1 斐波那契

斐波那契，一行秒 `return n == 0 || n == 1? n: fib(n-1)+fib(n-2)`

## 编程题-2 括号匹配

秒，栈就行了，\*号直接忽略

```js
/**
 * 代码中的类名、方法名、参数名已经指定，请勿修改，直接返回方法规定的值即可
 *
 * 
 * @param str string字符串 输入字符串
 * @return bool布尔型
 */
function isVerified( str ) {
    // write code here
    let len = str.length
    let s = []
    for(let i = 0; i < len; ++i) {
        if(str[i] == '*') continue
        if(str[i] == '{' || str[i] == '[' || str[i] == '(') {
            s.push(str[i])
        } else {
            let top = s[s.length-1]
            if((str[i] == '}' && top == '{') || (str[i] == ']' && top == '[') 
            || (str[i] == ')' && top == '(')) {
                s.pop()
            }
        }
    }
    return s.length == 0
}
module.exports = {
    isVerified : isVerified
};
```

## 编程题-3 最长递增子序列长度

做烂了都，dp就完事咯：[冲刺春招-精选笔面试 66 题大通关 day12](https://ysx.cosine.ren/cn/%E5%86%B2%E5%88%BA%E6%98%A5%E6%8B%9B-%E7%B2%BE%E9%80%89%E7%AC%94%E9%9D%A2%E8%AF%95%2066%20%E9%A2%98%E5%A4%A7%E9%80%9A%E5%85%B3%20day12/#%E6%80%9D%E8%B7%AF-2)

* `dp[i]` 表示 `0~i` 中最长递增子序列长度，每次在 `0` 到 `i-1` 中找可以与当前 `i` 构成递增序列的 `j` ，取其中最大的那个作为 `dp[i]`

```js
/**
 * 代码中的类名、方法名、参数名已经指定，请勿修改，直接返回方法规定的值即可
 *
 * 
 * @param arr int整型一维数组 数组
 * @return int整型
 */
 function lengthOfLis( arr ) {
    // write code here
    let len = arr.length
    let dp = new Array(len).fill(1)
    dp[0] = 1;
    for(let i = 1; i < len; ++i) {
        for(let j = 0; j < i; ++j) {
            if(arr[i] > arr[j]) dp[i] = Math.max(dp[j]+1, dp[i])
        }
    }
    return dp[len-1]
}
module.exports = {
    lengthOfLis : lengthOfLis
};
// 求数组最长递增子序列长度
```
