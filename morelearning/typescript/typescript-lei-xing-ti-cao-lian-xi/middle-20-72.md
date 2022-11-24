---
description: Middle题共72道，是类型体操的大头
---

# Middle（20/72）

## 题单（中等）

* [x] [2・获取函数返回类型](https://github.com/type-challenges/type-challenges/blob/main/questions/00002-medium-return-type/README.zh-CN.md)
* [x] [3・实现 Omit](https://github.com/type-challenges/type-challenges/blob/main/questions/00003-medium-omit/README.zh-CN.md)
* [x] [8・Readonly 2](https://github.com/type-challenges/type-challenges/blob/main/questions/00008-medium-readonly-2/README.zh-CN.md)
* [x] [9・深度 Readonly](https://github.com/type-challenges/type-challenges/blob/main/questions/00009-medium-deep-readonly/README.zh-CN.md)
* [x] [10・元组转合集](https://github.com/type-challenges/type-challenges/blob/main/questions/00010-medium-tuple-to-union/README.zh-CN.md)
* [x] [12・可串联构造器](https://github.com/type-challenges/type-challenges/blob/main/questions/00012-medium-chainable-options/README.zh-CN.md)
* [x] [15・最后一个元素](https://github.com/type-challenges/type-challenges/blob/main/questions/00015-medium-last/README.zh-CN.md)
* [x] [16・出堆](https://github.com/type-challenges/type-challenges/blob/main/questions/00016-medium-pop/README.zh-CN.md)
* [x] [20・Promise.all](https://github.com/type-challenges/type-challenges/blob/main/questions/00020-medium-promise-all/README.zh-CN.md)
* [x] [62・Type Lookup](https://github.com/type-challenges/type-challenges/blob/main/questions/00062-medium-type-lookup/README.zh-CN.md)
* [x] [106・Trim Left](https://github.com/type-challenges/type-challenges/blob/main/questions/00106-medium-trimleft/README.zh-CN.md)
* [x] [108・Trim](https://github.com/type-challenges/type-challenges/blob/main/questions/00108-medium-trim/README.zh-CN.md)
* [x] [110・Capitalize](https://github.com/type-challenges/type-challenges/blob/main/questions/00110-medium-capitalize/README.zh-CN.md)
* [x] [116・Replace](https://github.com/type-challenges/type-challenges/blob/main/questions/00116-medium-replace/README.zh-CN.md)
* [x] [119・ReplaceAll](https://github.com/type-challenges/type-challenges/blob/main/questions/00119-medium-replaceall/README.zh-CN.md)
* [x] [191・追加参数](https://github.com/type-challenges/type-challenges/blob/main/questions/00191-medium-append-argument/README.zh-CN.md)
* [x] [296・Permutation](https://github.com/type-challenges/type-challenges/blob/main/questions/00296-medium-permutation/README.zh-CN.md)
* [x] [298・Length of String](https://github.com/type-challenges/type-challenges/blob/main/questions/00298-medium-length-of-string/README.zh-CN.md)
* [x] [459・Flatten](https://github.com/type-challenges/type-challenges/blob/main/questions/00459-medium-flatten/README.zh-CN.md)
* [x] [527・Append to object](https://github.com/type-challenges/type-challenges/blob/main/questions/00527-medium-append-to-object/README.zh-CN.md)

## 解答

### 2・获取函数返回类型

* [接受挑战](https://tsch.js.org/2/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBBMELQUO3Bg15UL+KgHU0Cvxg9tUN4+ho9UnjhNKICMBPCAQQDsAXACwHs7qAxAVwgAoABAIaMAZlwCUEAMSBaOUCS3tICWdEQFMATtPJdFAGwZxlRIlNMRAGRmA7t2NRAsHKB-eUAUrhAAGAJVUMu6ugBVKAA6qLhCAedqADc4Q-kEAygDG6ooBDBCAIW6uHl4+0aoAPL4AfCGA2zb4gEAMNhCA0fKAQZqAWP+VLk0MAM5EcWwtKSJ0EAC8fABuAFwQ5CwsuqrCkn0FEADeRFCKIkPiy1AQ6p7evQCMm6q6LaqbUDtZvdBEAL6VDIGqEIL9EACylJl7ObmPQSw1j15sBgBBACl6gArjQA-2oAvxQgACJ9hAAD4wBFEJouSrzQAU6hAAOKKZhccgQQBQcoBT80A0O51JgMBgBFrDUGtOJMAB0ACsWhyWOoAObAaDAABeTDgAGEAHJgEDAMBgUAQAD6avVGvVEEABvKpQDHcoBAD1VmpNKog8sV-2en2+2Se+XmA18EFUAA8GKo6AATFp8Dn+wSC5nCSgAbQAurN5so1Jo3BAAPwQNyjOiqQYaRXK00miCAaVtAKvRjiqxpzWotigAtgF+SkrYsIABRACOXEEugANE3XUE4ilbhAROoWJWIAByfhWuDs9tTOgC1QtYBcBh6Fpjy1PCBxQSnX0DUNERs91R93Ittu6XJdRLzrs23Z2oK5XhRiA35QCgrfjtHk9ni921yfZoAAZnvL5Hz8e1X36eYQNA78Cl-KBj17Bhz1bIDJRHAIpldAB5cguVPBgINtaDn1guYIBw6t8KIki+yQlDu3QzDL1yAAFYdK0UU5cnGSZpjoZCPkgq5fmo+YeJHfi8iEqZhCQ5C-3YwCr2k8cRAmMdyKgqS3y0scdJYMcWLU0iOKA5E0WgfTJPtK1AUHUSf0sgCsKvWyYAcn4nKeFyen2Czw03IJaNwhjiNIt4ligQRRlDECuxM3SwqgchA1GMcmGOXQzKIAIdkGV9Uy4StyEze4wA6Ogulct5eBGMYJiUug30GRMIGRUYbjqhrgqalrFJErsAHdRhDTrut6mAsxAUsyzNQBoOUAADlAFNrJay3NBVQCIeZADAlQBquV1QBjyMAFW86QZJkWWANlOR5PlBWFYBhBacaNDFCUZQOiAaUu67GWZVkWnZbleX5IURRaSYV0UTo-sAF7NACxNKwgdu0HwaeqHvqlWULTAIA)

不使用 `ReturnType` 实现 TypeScript 的 `ReturnType<T>` 泛型。

例如：

```typescript
const fn = (v: boolean) => {
  if (v) return 1
  else return 2
}

type a = MyReturnType<typeof fn> // 应推导出 "1 | 2"
```

正确解答：

```typescript
type MyReturnType<T> = T extends (...args: any[]) => infer R ? R : never
```

注意参数数组\~

### 3・实现 Omit

* [接受挑战](https://tsch.js.org/3/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBDMELQUHnagG5wgeQLYEsAul5yFH4BGAnhAIIB2OAFgPbUUBiArhABQACAhrQDM2ASggBiQLRygSW9xbalibiSbLABsccLNXz4xeiIAyMwHduOqIFg5QP7ygClcIAA0y5bSVABUyABwCmAZQDGAJyx3HAhAELc7BxwAHhcAGggAaQA+J0Btm0Bo9UAgBlMI7BwnQCx5QGwlQC+9QAA5QCo5QEB3QFNXOwSnCUB1bUBW63DbFydAT+1AQxjsqHxAaPlAIM1ALH+c20mcAGd8LRxPfwFeX08IFwYAEwYIAG98KBxcVU8ALghpnEDqAHMDiE3PaYCgo6Zzy+u7qChfBgx3CcFptziQGAwTvx8ABfHI4DxrDbbAAK-k8ADcsJ4AO4QAC8EAAsmRIjEtgx4gByR7PQLBBTUSkQAA+EEpRxwJ0pSRyf2olwgOHJ5yRDFRGKxuIJ+x+ED+AKBnhBEGWqmmnliMPwk1sOSSEEAFOoQADiuDobBIEEAUHKAU-NANDuozoOBw7mmp2AwBmvjoADoAFbTH0Mfw3YDQYAALzocAAwgA5MAgYBgFOgCAAfUzWezWYggAN5UKAY7lAIAeGZz5fTECTKfhXiJJLyMXiCQgngAHgtqJtphAANaeMgMATrfXS-AAbQSA4gWj7A6H6wgvB7U4o7c73cSEAA-BBqBjFhBzquALoiycDk9gWFgNMV8sQQDStoBV6KsgzL99z1awAODIVray7BAACiACObC8Ko8TAW2Xi+CE0Iqv4-xstwAFwN6kEnLcTzAGwRxqpSYAAXKy5PPiEDjvgMFwdEYEQaoUQ0Z48FKgAjPExKkqKVI0i89JMNySRJJqUDMfBTHgZBTGwSxwIAEycQ2uBktsvFPPxbyMiybLyoCnjAkJIlgFet7ABAaHTHA7a0dZ-jIf4xEIq29nBhRXGNjxbJ8XSWlMqylJaOikFYJs3IpvMizLKs6zkns+AcicHxXFo3wPBpvkMslXz4HpirKmCEKeFCN6RUsKxrOJwJsfFhzHGcFwpbcuX-PpwKguCkLaKVtBRRVIGyaxmzybVgr1dlqXXqmIAfp+laANByZSAKbWs2flWyagPg+qAGBKgDVcgWgDHkYAKt6Os6rrup6zy+gGQYhmGwD8NM2KLJG0bxltED2sdp0um6HpetdgbBqG4bTBC+EMrMUD6oAL2aAFiaxg-ed-1Xf6QN3VGsYJtWYBAA)

不使用 `Omit` 实现 TypeScript 的 `Omit<T, K>` 泛型。

`Omit` 会创建一个省略 `K` 中字段的 `T` 对象。

例如：

```typescript
interface Todo {
  title: string
  description: string
  completed: boolean
}

type TodoPreview = MyOmit<Todo, 'description' | 'title'>

const todo: TodoPreview = {
  completed: false,
}
```

正确解答：

```typescript
type MyOmit<T, K extends keyof T> = {
  [Key in keyof T as Key extends K ? never : Key]: T[Key]
}
```

乍一看很绕，其实搞懂 keyof 和 in 就明白了。

### 8・Readonly 2

* [接受挑战](https://tsch.js.org/8/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBAcELQQEoFMCGATA9gOwDYE8IAmSeOci0gI0IEFsAXACx0IDEBXCACgAFVGAMw4BKCAGJAtHKBJbwkAnNFjyFxmKgCtkAYwZwA1snwBnUqXHmIgDIzAd26moAPgiBGV0DsMYBlrQFeBgCqVA3-6BF6MAYf8Aia0A5+IgABUQIQE5TQG34-0AKWMB5xMAgBjsIQDztQAbnQAA5QCo5QCwEwApXAAMAWXwUDBwCIgAeABUAGggAaXsSgMBg7UAyPUBIc0ASOUBZz0BvH0Bo9UAQt0Ah5UAHUxKGksAYlRLWkrSoUhWSwHBjQCztQBS9QD7owDt-QC45KqUCCfmSicA9HUByA0AxtJTAIM1AHPNAKnNABeNAbPktgKATCV9oB-eUAAkZ9R6AX4TABvKp0AV8qAb+iAoBGHUA8wqAOzMCtcLjV8I0OjlAOwW6wgpEA0fKvdIlGkMExQACWjGQckEqC0yAgDUwWAgAG9SFAGAyGLhkAAuCBGBhyJkAc0FEHQyCMWllAAdhThJdLZdgFVAoFpMABbdVihjIdCSqiYTBigSkAC+6WN2GlEAYPMwkoquOU9W5WBaAHJhaLkCGIAAfCAh5WqjVa7AhxwAXn5ivDYslACIABKGXNNRUJtUMzUM7UQXOCO1UVByYuK41mi1WyVs3BGZAlqAujZC70AOmznIzBeQuFwmFzEGAwAgAFE5HJMHJJVoBNhMAwIApUEYjAy5dgIKh94o8RB1Wv1SyGPhSF6sMOy0mq2eJw25Gw7XOF2XVd103bdd0vQ9j1Pc8IMuQhb0we85EfZ8R1bc1kEtdAIAzGUOE5QCAHlWk2Gl0kcQAKdQgABxEUmA4KgIEAKDlAFPzQBod0ALH+mAYBh1SMcUFzpLQmGHdQjGHdc5WAaBgAALyYOAAGEADkwBAYAwE00AIAAfT0-SDP0iBAAN5CZAGO5QBAD10wybJ0iB1M0x97wgP0rwDRoWlaCBkAAD0tbB0CMCADHwTBBC5HDgsMMKuXTTMoAPOCIAAbVaQwICZNoAF1JQaVLDCysAnQgAAyCBCJNEUPLaewtJAazbIMiBAGlbQBV6KKckGsavT7I0hkzXXPcnM5PkIFoXAGQMFolx8+8dAgYrBDXE0414Ya4GE1Bp2QfUVWADhhW7ENHPwZytx7IKM2S0gZrmhg6nGybkDqVzqncoNMAARnsFp-QIRpvW++wfpu2btHux6DBeyo3NqAGsE+0MxyjWN4xVctKxwVNprBnQrWBvtl1xiGJqh164MDb0iCRkUxRRuN3wrZNsaJu78ZBwqwEAtajDgXy7r54C5DAYbvKFyLybxSmEZpiN6ZDJkADctoZdBU00plLVZdlOQ+z74s9WmJSlGV5VIRnMewAB+HVTf1Uh0Pba0IFte00GwIqNeZbWOS5KmDcS68x1tvUDSVdGPxwG2TdDh3TQwrCbTtB0PZdMBNZZNlfdu8GrQD2HCGDmOzYSgvw8TJnP2j3US4gR3MI7F3k-dz3NK5+ruqawBoORyQBTay67revb0hHEAMCVAGq5UzAGPIwAVby4ni+IE4AhJEsSJLkKSZIEIwAHcWTkhSVJHiB2Nn+feP4wTVVX8TJOk4AjHtA7P3pCBHEAF7NACxNGxz8Xq-hNErfDeB8lKqQcmAIAA)

实现一个通用 `MyReadonly2<T, K>`，它带有两种类型的参数 `T`和 `K`。

`K`指定应设置为 Readonly 的 `T`的属性集。如果未提供 `K`，则应使所有属性都变为只读，就像普通的 `Readonly<T>`一样。

例如

```typescript
interface Todo {
  title: string
  description: string
  completed: boolean
}

const todo: MyReadonly2<Todo, 'title' | 'description'> = {
  title: 'Hey',
  description: 'foobar',
  completed: false,
}

todo.title = 'Hello' // Error: cannot reassign a readonly property
todo.description = 'barFoo' // Error: cannot reassign a readonly property
todo.completed = true // OK
```

正确解答

```typescript
type MyReadonly2<T, K extends keyof T = keyof T> = {
  readonly [Key in K]: T[Key]
} & Omit<T, K>
```

结合上面的 [实现 Omit](https://github.com/type-challenges/type-challenges/blob/main/questions/00003-medium-omit/README.zh-CN.md) 和简单题中的 [实现 Readonly](https://github.com/type-challenges/type-challenges/blob/main/questions/00007-easy-readonly/README.zh-CN.md) 可得出该题的答案。

### 9・深度 Readonly ⭐

* [接受挑战](https://tsch.js.org/9/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCcELQUI+2gyvQgJQKYEMAmB7AOwBsBPSeOSq8gIxIgEECAXAC0PoDEBXCACgACWFgDNuASggBiQLRygSW9pAJ2z5i9KXhoArDAGNmcANYYSAZ2k4MGAA7lyUhxEAZGYDu3O1AB8EQIyugdhjAMtaAV4GAFUqA3-6Ai9GAMP+ARNaAc-EQAApoEICcpoDb8RGAFLGA84mAQAzuEIB52oANzoAAcoBUcoBYCYAUroAhbgAGACJW1pi4hKQAPAAqHvWRgMHagGA6gJ-agIYxtYDz1uWAQ8qADqaAU8qAboqACtrjgEgJgEr6gAzqgH3RgFxygFfKgN-R+VDkgBUGgPfKgKdygOIKu4AU6oAm1oCIxoAYRjKAiEaAN3KAo3KAEE1AGAu41yc0AI36RQC-inNIoBvHzkgF+EwAHpoAAdMAwAGARTDcoAxeUA9GaRC6AWblAGyOt0qgHH4wBhkYA1t0AvDpXQC-AYAsTVqgFg5QAwKoAJC0A0fKAU3MPoFAI+6Zwg5B5gCDNAr1GXMUzkZgkawYCAADQgAF4IABvMVQKAADwAXDq9fqoFgTQBGcjmmgmgDkrAAlg7bRAAL7ukiO1gmN1QL3nKCK5UQACiBuV+gwOE1pvdynaaggxoT5qgSdUpAglogNozECzHXo9ogTtd7qD+uLKZ95b9JAdZurCqVKu6eHw8eaNja2ZInVVXmAwAgpnY3CIcZoKtMWAAtiqsOZ6pHo8xY-VyDLt8GIF5HhAAOLOtjcGgQQBQcoBT80A0O6ALH-WMxmNZTEbR3LdKwAHRaUw-ngigAObANAwAAF6sHAADCAByYAgMAYAoaAEAAPqYVh2FYRAgAG8rUgDHcoAgB4YTh5HoRASEoaGKq9q0Kglj0EAYAam4EDg5gAPLaHozBeFq2rkLWOYANoANImBAzoEBAxgkHgIgQN0AC6JrdBJJgqSxbEYBx5iYLoQE4J0wgkAANLmBAkB47oAPzKZpJDaax7GcRAPAEPozqEO6UAORpknOX5EAmvR-ZMYFWm2ea6lOSpYBemAaEUeRECANK2gCr0dUPJkaluHUc6C7WEBzAQLRprhgAjtwWBEJZ658Z6EAiIoeALuWAi0XA351UQenARgpjANwzDOkQphumAFW6CuQ3xqJ5CNfonTVbVRCdOFjFqEOHgNVGfGxh4e1gAl03tmq8ZCRaJp8JIGpeAATI9tAmqYzCKDJwHkLoJrXfqOAmjQeB4P1wjuhgf0hcBUOFlArCw3DUDOiaH3cBgIXmlojrvZ9BDAQGcPVoWhi+hgRBEHghPmsT+pECai1IxWDrmZjOps1AC4M06-oJUjHqs4WfP6tWXpehVy2bnGgnCdtOZ5ndmpPS9mZy6Wb0fV9svJjmv3s+aIn0IDEDA6D2AEImassYjBtWzD+tw4bEAIw7SNOyj5WKOjHNFlb2PlrjX3UxmtO2zr9Ckw25OU8HgYhU79O++HECM3DzOC3D-1u1bXNJwOKc802wuFgLIXF565BiyhqEgHl+WUYA0HKlIAptZ1-lVHIaA5BeIAYEqANVyBGAMeRgAq3k+L5vh+wBfr+-6ASBYHAMIpgAO4YIokHQfB3cQPeI9j6+76fqY35-gBQGgeBpig6NPkEPKngQIAL2bMq4+8T0fJ+z+fG+wQh1FgEAA)

实现一个通用的 `DeepReadonly<T>`，它将对象的每个参数及其子对象递归地设为只读。 您可以假设在此挑战中我们仅处理对象。数组，函数，类等都无需考虑。但是，您仍然可以通过覆盖尽可能多的不同案例来挑战自己。

例如

```typescript
type X = {
  x: {
    a: 1
    b: 'hi'
  }
  y: 'hey'
}

type Expected = {
  readonly x: {
    readonly a: 1
    readonly b: 'hi'
  }
  readonly y: 'hey'
}

type Todo = DeepReadonly<X> // should be same as `Expected`
```

正确解答

```typescript
type DeepReadonly<T extends Object> = {
  readonly [Key in keyof T]: T[Key] extends Record<any, any>
    ? T[Key] extends Function
      ? T[Key]
      : DeepReadonly<T[Key]>
    : T[Key]
}
```

递归解决，注意特判 Funtion 的情况

### 10・元组转合集

* [接受挑战](https://tsch.js.org/10/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMAMEFoKGFFQI36Bt4wECqDG0yiEGF4BGAnhAIIB2ALgBYD2V5AYgK4QAUAAgIa0AzNgEoIAYkC0coElvcQEsqAgKYAncTTYAHADaLxbKrKZ48Y0xEAZGYDu3Y1EB52oAbnQNs2gaPUABgBVNO9wwCqBpgAedwA+V0AYf8Bg7UAV+MA9tTRAASNASHNAHgVAELccQCAGGwhAaPlAIM0c12KaAGc8GlINXQplVQBeCABtAHJoFoAaCBaAJk7ugGYWgF0cyuqId0VSmghGz21FH39DKkDa5RCIYGAIRQAPaoBjGkUAEwgaBghiXTaWiAAfbr6nwZa8YtccrcAKdQgAOKyehsYgQQBQcoBT80A0O6ALH+6DQaBpSgAuHZlI50AB0ACtSliGMoAObAODAABedAQAGEAHJgEDAMBgUAQAD6HM5XM5EEABvJpQDHcoBAD3Z3LFbIgjOZ410C28fgCa1Cc0me32pyoZ1KzXkSlUADUuljjbqVBAAErTGjDAD8EH1bzlSwVq0ClpmIRRECoigAbipmazxWKIIBpW0Aq9GACldcqLgzypbIALYaQmzGUQADeEAAogBHNi8LRdbOHRQnCAAXwgAmUDET3W4MoQmMLOioROmwDYNFkWlKHzA6aOvFK0xVTTwJeONECeYLWmCXmdKyCTWgPQGXRaABYAKwANn6NGUbEUwxCXXXAzeO4PD2ex9PIQvk9LJ1n+cLi8Wy0VgTXG7npeG7Ph0YCjCyICxnGEqANBygAAcoAptbQXGkpMqAeBbIAYEqANVy-KAMeRgAq3vCiLImiwAYtieIEsSpKwMA-ClAA7ioFJUnSmEQDCREkUiqLoqUmK4vihIkmSpQMFo3arOUUBbIAL2aAFiaVi8WRAlCdRolsTS9JSmAQA)

实现泛型 `TupleToUnion<T>`，它返回元组所有值的合集。

例如

```typescript
type Arr = ['1', '2', '3']

type Test = TupleToUnion<Arr> // expected to be '1' | '2' | '3'
```

解答： 没想太多的递归实现 👇

```typescript
type TupleToUnion<T> = T extends [infer V, ...infer Rest] ? V | TupleToUnion<Rest> : never
```

翻了翻 issue 发现的另一个实现，确实哦！

```typescript
type TupleToUnion<T extends any[]> = T[number]
```

### 12・可串联构造器 ⭐⭐

* [接受挑战](https://tsch.js.org/12/play/zh-CN)
* 我的解答

在 JavaScript 中我们经常会使用可串联（Chainable/Pipeline）的函数构造一个对象，但在 TypeScript 中，你能合理的给它赋上类型吗？

在这个挑战中，你可以使用任意你喜欢的方式实现这个类型 - Interface, Type 或 Class 都行。你需要提供两个函数 `option(key, value)` 和 `get()`。在 `option` 中你需要使用提供的 key 和 value 扩展当前的对象类型，通过 `get` 获取最终结果。

例如

```typescript
type Chainable = {
  option(key: string, value: any): any
  get(): any
}

declare const config: Chainable

const result = config.option('foo', 123).option('name', 'type-challenges').option('bar', { value: 'Hello World' }).get()

// 期望 result 的类型是：
interface Result {
  foo: number
  name: string
  bar: {
    value: string
  }
}
```

你只需要在类型层面实现这个功能 - 不需要实现任何 TS/JS 的实际逻辑。

你可以假设 `key` 只接受字符串而 `value` 接受任何类型，你只需要暴露它传递的类型而不需要进行任何处理。同样的 `key` 只会被使用一次。

**正确解答**：注意 Key 必须为之前没取过的，或是 Value 类型与之前不同的（用例 2 和 3）。

```typescript
type Chainable<Obj extends Record<string, any> = {}> = {
  option<K extends string, V>(
    key: K extends keyof Obj ? (V extends Obj[K] ? never : V) : K,
    value: V,
  ): Chainable<Omit<Obj, K> & Record<K, V>>
  get(): Obj
}
```

### 15・最后一个元素

* [接受挑战](https://tsch.js.org/15/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMCsEFoKABzQcCqAA5QVHKGFFQBL6UQSOIICMBPCAQQDsAXACwHsbKAxAVwgAoABAQ3oAzDgEoIAYkC0coElvSfwBOC-uQIEJGiIAyMwHduaqAD4IgRldA7DGAZa0BXgYAqlQN-+gRejAMP+Aia0Bz8RAAKAJQiBOU0Db8Q6AFLGA84mAQAz6EAaAFOqAJtaAiMaAGEZSgF96gHXRgP7ygBSuACrkAA4ApgDKAMYKAJb5dBAALAB0AAyRgHnagA3OWIBYCVkABgAy-ADOdAA8OQY9joDB2oClxoDryliADqaAI349OT2AbnqAK-GAe2qAbopoWHiAIW6A3j6A0eoRUASA0fKAQZqRPU90gwR0BYUQigrQEAC8EAA2gByfjAgA0EGBpAhUNKwIAum8Pl8lAAmf5AgDMkLRkOgSOuUHeRQgdH4FQANr8AQNhiNvtAjMBgBBCgAPIqlOiFAAmZKYEFIn2B8ORpPJVIxtKGo2+aOZrI5XJ5-LoguFMAITx6kSM0QgAHEKowOKQIIAoOUAp+aAaHdAFj-DDodHygwAXCyXqUGPUAFaDepMBQAc2AcGAAC8GAgAMIAOTAIGAYDAoAgAH0M5ms5mIIADeWOgGO5QCAHuns2W0xBE8mSZ86aMcmz2TyaLzBl9WICEUYAQ2Oc3W0D6kOKjQhIUFBAvIVhpCR2OJ30ERAAPwQPoQV0QGiFABu4+TqfLZYggGlbQCr0VkbqWjzmqxUALb5QM1GsQADeEAAogBHDj8SmQp+nKFNyEAAL4QEIChMPeUK8DWCBev+lKFDQQbTsAHB0FSgzAtWKKlEM06YoCBBASqIw-n+lIjHWIyAjiEB4jAXb4gYBjgmRwHcpRv7-rRsr0dw4h-EY0BooxH78JuwyVGh4Gse+XwyXQclBuB7GcUiKYgNeN4VoA0HLoIAptZ6TelZJqABBGIAYEqANVy+aAMeRgAq3g6Touu6wCet6foBsGoawMAgiDAA7uOEZRnG1kQLaLluc6boeoMXq+v6gYhmGgxMJSWEVCwryGBAgAvZoAWJq6PFHlJSlvnpRFMbxlWYBAA)

实现一个通用 `Last<T>`，它接受一个数组 `T`并返回其最后一个元素的类型。

**正确解答**：基本送分题

```typescript
type Last<T extends any[]> = T extends [...infer Rest, infer L] ? L : never
```

### 16・出堆

* [接受挑战](https://tsch.js.org/16/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMBsEFoKC-FQYBqUQr2MCMCeEAggHYAuAFgPYmEBiArhABQACAhuQGYMCUEAYkC0coElvQewBOE9vgwYBCiIAyMwHducqAD5AFOqATa0CIxoAwjIYC+9QHXRgf3lAFK4AVfAAcApgGUAxhICWdshAAsAOgAGdQhAPO1ABudAADlAKjlALATLAAMABSo7AB5rDXjAGH-AYO1AUuNAdeVowAdTQBG-eOtswDc9QBX4wD21aMBGVzKK+MAQt0BZJQAbBxIAc0oEaEBPDMBTuUAPt0AYFTbALwzAeL1SwAQjNrLAIAZgwGj5QCDNYPi9sgBnDDJ7BwhJCWgIAF4IAG0AcnYHgBoIB9xX95cvh4ATB4AXWOp3OUgATDd7gBmN7gt7QYFQEGOCASBxXW7JNIXaAaCDAYAQBwAD0cLjIDj+EDIVAguDOj2ebw+vx+SJpoPRkKxKVSF3B+MJxLJDgpVJpdIZMLhHL28WCIBAgFyMwBomkrAFj-k0A7BZZQAVBoB9OUA98qjcLxJwUdxcMjZJIMA4UeKAGJV4gBVEgOq02wDoKoB8f+C+K0EAA4u5KAxcBBAFBygFPzQDQ7hqKGQyHYDgAuQmHFwUPwAKwOfioEj6wDgwAAXhQEABhAByYBAwDAYFAEAA+h3O13OxBAAbybUAx3KAQA9292x22II3mydUdj0iLKSQ-gdzrQ7oD8bdrAvesv7n4D+4SFwHBIIAAlBwHMhvI8ns8AGUBEAA-Ber940xBrGAZ2dEvaFDzqSi57pw+Drm8RBSDuS4ruB66bvuB7WG8B5+NBEjAn+EAWl6wEkqB8FrhuULbiBu4rncd6nhAdBoYex60Ze17Pm+LGft+v6gu6nrWgRRGrhBgJQTBFFwUJiFQncEDoZhLzodYwItiAo7jl2ECANK2gCr0ZYGxqepHaTk27gALZ2EW3g4QA3hAACiACODDsF0bx2aKFIQAAvhAXASFQpnvKwf4INmLk9P0V7AAwZDuF0BwPNOoIuOwBxXtJGDueSZCpI5zldKkc53LCEDwjAG5vMVsoaBoLyZR5OV5S5hV8kyvyfCyPwsgCFX3E87VskCNV1VAWVio1TnNUVvWIbV9XZblk0FQBDqpFVpUIiJ9w+G8ACsM0lWV0BvDtED7cN83jYt+WFYBa1bYhlUbnNo0NddzV4fx61HTNP0Xa9C1NQVn05Y99zPSN9lvUDqS8ZaX2HZtlWnedyN7W8iPlf9UOA0tsMevDoMPTNENgMpraGRpgDQchEgCm1gZhnGSpGD4oAYEqANVy-aAMeRgAq3omyaphmwBZjm+aFsWpawMAnAHAA7qeFZVnWLMQPGvP8ym6aZgc2Z5gWRYlmWBxUF0MXuDQRyaBAgAvZoAWJqqBrgva7rYsG4rNb1lOYBAA)

实现一个通用 `Pop<T>`，它接受一个数组 `T`，并返回一个由数组 `T`的前 length-1 项以相同的顺序组成的数组。

例如

```typescript
type arr1 = ['a', 'b', 'c', 'd']
type arr2 = [3, 2, 1]

type re1 = Pop<arr1> // expected to be ['a', 'b', 'c']
type re2 = Pop<arr2> // expected to be [3, 2]
```

**额外**：同样，您也可以实现 `Shift`，`Push`和 `Unshift`吗？

**正确解答**：看了小册后不难做出

```typescript
type Pop<T extends any[]> = T extends [...infer Rest, infer L] ? Rest : T
type Push<T extends any[], Arr extends any[]> = [...T, ...Arr]
type Shift<T extends any[]> = T extends [infer F, ...infer Rest] ? Rest : T
type Unshift<T extends any[], Arr extends any[]> = [...Arr, ...T]
```

### 20・Promise.all ⭐⭐⭐

* [接受挑战](https://tsch.js.org/20/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBBMAMEFoIAUBOB7AtgSwM4FMA6AQwBtTJEFqbKAjATwgEEA7AFwAt1WmAxAK4QAFAAFiHAGYCAlBADEgWjlAkt4LiqVMSbyADhhwFKleSYiAMjMB3bkagA+CIEZXQOwxgGWtAV4GAKpUDf-oEXowDD-gImtAOfiUACUIQE5TQG34n0AKWMB5xMAgBmsIQDpUwFNFQF-FQAdTAAM0LDx8ZnIc30Bg7UBS40B15XyDfAAZbABrfEBP7UBDGKzAEb9fQBX4wD21QB4FQBS9QC45PP1CgB4AFRtSwDdFRRyZnMB6M0BjyMAE80AQt0Blv0Ac826kqEoc8-ZcSgBjHlx2CD0CggBGCABeFEmCQlR8XHQpAAbvhhABmGQAbhudweTzq0A+EAALNBoVBbqx7o9vvgwUjWPgAO5fZ74Kb3VDYVgAcxswmEfwBwPwABoIH8AFb4a7sOTvOwAb0oUAI7Bm2Ew+HQAnYjP+gJB7JesFg7IA5JJ0Oh1VDKABfPWnKDAYAQfAADx0PPY+AAJhB2OgIHR8BAJmSpgBtVgCTCu1Ds1HsynUmkAXXmMKxcKRtUKxVIwi98MKL3ZqYI0AzuLB4YgxFwEEx9xkZ3OyTsgAp1CAAcWwXAEdAggCg5QCn5oBod0AWP+cdjsHS4ABcpsu104hE5uEI6FQNOAcGAAC9OAgAMIAOTAIGAYDAoAgAH0j8eT8eIIADeR2gGO5QCAHofTw+DxBt7u7TzSOo3dJWLzsDxSXUiZTMws5FpatqsHaRZ-MQdo8KQTACKwTSsOgRKsF6kbCJQQJkAI-yDhy+CwfBTBeoQFEgTSuDhqyYAyIR8YEFMgoQF6ADS+BMNSEAtAw6CSCwoHhoRVG4BxXH5uB+CQUWTHktSkj4KgEAAGp2AA-GpECiaBEkMPm+o2Lu+6Pg+ECANK2gCr0YAFK6ANHy95mWeL6SjoM4POwDDWhArEAKIAI4CGQ7K+VaNoQPqECSPoEDqqInnWggY5kKQMk0v8wCytgpC4Oqu4lnCuKJjM-zsG8nzyYmybpjA7J5gWRYFWWBU4mSxWlYiFVFeQ1XstmAGFL8CosuCMj5oWxaws1sKtYB5Alfc+JdW1PVejV-XyUNzIgqN4ZlmACVutchb-EiXqUKF1q8lMAVBaQUyHQJs0JvNpU1fJ3rrXVkY2DYdFQJdNo3YFZAPV50qCZmRSvfcG24p9fXsr6-rKT9f0XWF123aDj2Q91pALewYLsh9Pp+gGSPk8plMo6gaN0eGJkgI5TlPoA0HKAABygCm1izTnPjuoCUHYgBgSoA1XKXhsgAq3j2fYDsOwCjuOk7TrO86wMAEi4ESylLiuG5CxAnZSzL-ZDiOuBjhOU4znOC7MlldwG4AL2aAFialgm3L5uW8rNu62um4vmAQA)

键入函数 `PromiseAll`，它接受 PromiseLike 对象数组，返回值应为 `Promise<T>`，其中 `T`是解析的结果数组。

```typescript
const promise1 = Promise.resolve(3)
const promise2 = 42
const promise3 = new Promise<string>((resolve, reject) => {
  setTimeout(resolve, 100, 'foo')
})

// expected to be `Promise<[number, 42, string]>`
const p = PromiseAll([promise1, promise2, promise3] as const)
```

**正确解答**：

```typescript
declare function PromiseAll<Args extends readonly unknown[]>(
  values: readonly [...Args],
): Promise<{ [Key in keyof Args]: Args[Key] extends Promise<infer V> ? V : Args[Key] }>
```

疑惑吗？疑惑就对了，请看看这个 pr ：[Variadic tuple types](https://github.com/microsoft/TypeScript/pull/39094)

### 62・Type Lookup ⭐⭐

* [接受挑战](https://tsch.js.org/62/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?ssl=33\&ssc=1\&pln=34\&pc=1#code/PQKgUABBBsBMEFoIBUCeAHAphAMgezwGsBXdSRBSq8gI1QgEEA7AFwAs8n6AxYiACgACAQ1YAzYgEoIAYkC0coElvWcSYBLTrIC2wslHIyDEQBkZgO7dy5QJDmgN9NAMP+AKg0D3yoF+AwDB6gbHNAnBaA7Y0AL5oCo5QD0dQHIDQAp1QBUAwAgVQG8fQGj1OUBT80A-I1jAIAZzKBDAE2tARGNADCM5G0BEI0AbuUBng0AsBMBx+PDomIADAGFhFggAHwgAETwAczq5QBwTQCJfQBtFQEdFOpYMTDrAdW1AVutAU3NAduDANeVAD7dAFL1AELdUwCNjQFPlQF3owBfomxDAU7lAaDlALk9AaPkCksB8czc6-CIAVXQAHi7utogmiwADQQADkABMeqCAHx1JaAdP06r86jZXgRCJ8fj1-oCQaCAMbNGFwxGAuppPRQOrUlgAZ3IqlYmAATmJhPjsICIABvchQSZYABcYMJLFBfIgNGZmEw4NpwtBDDotNpjNUolB-1BAGUOMz2MJVMzNe1QQ1iMyADYmsEAIUwTG6wmt5AAvukIIyWCy2RzOtjeVB+VMFZDuuKg5LpbL5WCABJ4FTgm2g23M1QsFiiVAp23ES2WsO5vAADxZEaD+LwlrwzIVUrwAHcmCnG2wM5gUzRLezCBX3ZSIALsABZVC-CAAXlw6MxXPavzxRehEGAwAgmBLWHx3vBQ7wkuwSJ6dXI1NPg5XIQgAHEM2xiDQIIAoOXigGh3QBY-2xM+h5Wu6fibAAHQAFa0kBtbdMAcDAAAXmwCANAAcmAIDAGAGGgBAAD6uF4fheEQIABvJbIAx3KAIAeOEEdR2EQGhGHDjOHzfO8ILIBuJbekwcoQLSLDpo6K7Tu8HFcTx3JDiGnpMGILIQNqECuhAABkEAAEqYFWzLgl82YgtmK4APwCApm5ibSKAQMZ7zCkwmAAG4stIEC2Q5LIYWAWE0dRECANK2gCr0YAFK63FR3mEfRqiaOgtYtIxEkAKIAI7EM6ILxVumktEpYjMngmhgoIw4IIBzqWg63SYLSwDECwqiWrS4pgF6PrspyzQ8uQw4KqKFZSjKcoKkqqAqmqGparqMVsIaxpauaVq5uVzriu6TVMqyrX+n8gaSUKYJFrQ0YDfGibcbm6aZtmub5oWUJarapbluQVY1nWYINs2rbtt6XY9vifZgCtjHMJFzpTgC7ULj0DFTBAhK0pVYMANrkOl24sF8SUpZaXxvBi3zA9olpLlC0Igr80KkyjGU7hjyXOjjs742ohN4j1pPgywFNAmAAC6HmeSAoVhbRlyAABygCm1kLYV0ehoDkCugBgSoA1XIkYAx5GACreX4-n+wAAcBYEQcyUEwaItKNiycEIch8sQO+Gtaywv6Cv+tKAaB4GQdBsDALS1Y1eoTD0lAK6AC9mgBYmqYDtOy7bsG578GISh9FgEAA)

有时，您可能希望根据某个属性在联合类型中查找类型。

在此挑战中，我们想通过在联合类型 `Cat | Dog`中搜索公共 `type`字段来获取相应的类型。换句话说，在以下示例中，我们期望 `LookUp<Dog | Cat, 'dog'>`获得 `Dog`，`LookUp<Dog | Cat, 'cat'>`获得 `Cat`。

```typescript
interface Cat {
  type: 'cat'
  breeds: 'Abyssinian' | 'Shorthair' | 'Curl' | 'Bengal'
}

interface Dog {
  type: 'dog'
  breeds: 'Hound' | 'Brittany' | 'Bulldog' | 'Boxer'
  color: 'brown' | 'white' | 'black'
}

type MyDog = LookUp<Cat | Dog, 'dog'> // expected to be `Dog`
```

**正确解答**：第一反应如下

```typescript
type LookUp<U, T extends string> = U extends { type: infer S } & Record<any, any> ? (S extends T ? U : never) : never
```

翻了翻 issue，很巧妙地[一个解答](https://github.com/type-challenges/type-challenges/issues/149)如下：

```typescript
type LookUp<U, T extends string> = U extends { type: T } ? U : never
```

### 106・Trim Left

* [接受挑战](https://tsch.js.org/106/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMAMBsEC0EAqAnAlgWwgGQFMAzAF0mSUqvICMBPCAQQDsSALAe2YYDEBXCAAoAAgENWRPgEoIAYkC0coElvOSQLYADgBtRqpJsyr0ozeXKzzEQBkZgO7dTUQHnagBucIAAww5CpADyoAfC4hAGH-AYO1AUuNANlNAOw9ALO1AELdAdW1AMm9AJjlAbx9AaPVANz1AFfjAPbVAADlAKjlABtMElMDAN0V5Yryy5MACJUATNMAwuUB85STkwAB9QBZNWMAvL0BfNw7AIAY7CEBo+UAgzTGXWZIAZ3ISOnUCCBIsbAIAEwgAXjRNzxIvAHIoAAkCTU0OCAB1DnRNXYhT3whgYAhAFL1ACuNAD-agC-FN5XG53R7PV6ncizFxjD6ACnUIABxAxsPg0CCAKDlAKfmgGh3QBY-2wSCR1PMAFxfBYAYzYADoAFbzelPADmwDg8GAAC82EgAMIAOTAIGAYAloAgAH1ZXL5XKIIADeVigGO5QCAHjKFdrpRAxRLlqsIABldSiGlrA7nc4AHzeAB1mLaHSQYYa1u5sMcvMaIAQAB6qZjbeYQeYbTDMNkfA6+gNBkOuAAkAG9TeaCABfVORogEdAQIUEADuxszAQA-IcPMQTkXSx8KSbJSAtTr5RBANK2gFXowAUruM2+3ZXrxTh1E8SOsVmsUxAAKIARz4xgANPP-asaZPMxAiOgOLhTsJ3Ug6cZNAQowR5sA+CRMJp5jCwO6IDTRPNr-sIABtchzjcCC3LxF2XTQfCOWsznDdB3jXU4YPeXwV3-QDgNA4wIJrbxzkQ5C3jw5DUM3E4MPAz1vXOKAoDw+DCJQqAAJIkCl0wiioKo6iYOoqA4IIjYeLeXwiMYtDSNY8jIJw6jHXtSciA4O4aFEAs+NOBSlJUoSRPXZiyKwr0OLUpCGN0oDxLAgzKIgWTXXw04TLAABdFtByHCBAGg5fJAFNrNz2xHMBQHID5ADAlQBquRVQBjyMAFW9iVJckqWAWkGWZVl0A5LlgHEeZi3zXl+WFYKIAJGK4rJSlqXmOkmRZdlOQQYB5g4TQ70wLhFigD5ABezQAsTRsMqEsq6rUrqvlBRFfUwCAA)

实现 `TrimLeft<T>` ，它接收确定的字符串类型并返回一个新的字符串，其中新返回的字符串删除了原字符串开头的空白字符串。

例如

```typescript
type trimed = TrimLeft<'  Hello World  '> // 应推导出 'Hello World  '
```

**正确解答**：非常经典的[模式提取做匹配](https://juejin.cn/book/7047524421182947366/section/7048281581428932619)！

```typescript
type Space = ' ' | '\n' | '\t'
type TrimLeft<S extends string> = S extends `${Space}${infer NewS}` ? TrimLeft<NewS> : S
```

### 108・Trim ⭐

* [接受挑战](https://tsch.js.org/108/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMAMAcEC0EAqAnAlgW0spBheARgJ4QCCAdgC4AWA9leQGICuEAFAAICGtAMzYBKCAGJAtHKBJb3E0AptgAOAG17ykyzPPS9lePGMMRAGRmA7t31RAedqAG5wAGGHAB5UAPluAYf8DB2oHozQABygKjlAdW1AMm9AJjlAbx9AaPV3QDc9QBX4wD21AMAG0xDQ90A3RQlAEjlAe69AELdALy9AXzdgwF+EwCfdQGqIwAIlQBM0wCAGCwhAaPlAIM1m2y6aAGc8GlJFOQgaLGw5ABMIAF40MccAcigACTllZQYIAHUGdGUpiAWXCGBgCDkADyGAY3kpmk3iYYXV9c2dvYmFvC7bZuPABTqEAA4lo6GxiBBAFBygFPzQDQ7oAsf7oNBoih6AC5Tr1rnQAHQAKx6uN2AHNgHB4MAAF50JAAYQAcmAQMAwGzQBAAPrcnm8nkQQAG8vlAMdygEAPLl8yWciAstkDIYQADKil412GsyWSwAPocADpUbV6mjfeXDBzYAAycgENEcivOF3kVAmPQgPVGmCoJOOs3tlydLogtgAJABvZWquQAXzDnoEcnQEAZcgA7oqo7YIAB+OY4K02xzJtPHdFKsCm3PYABKmBJyLtDoDrvdWC9PqVjbkztdIdDcYTSdT6bDEbVGezlfztqLipLZYr5ob-q7gZbnu9M0n1tt5prddts5cbLAHKlkoggGlbQCr0YAKVxaErP-NlOEUuxoI0Gw1DEAAogBHNhdAAGl-K45FuCAowgAR0AYbBDm4U0kBxXRlC7Ek5B6YA2BoTBlB6b5y0-CBrl4HpMM3ABtPAfzA25HH-QDlGceYFhbI4QLY0YjhcICaLo21GN0FinCWdjeMOcTeP4m5BIA4TFyWKAoHEzipL4qBaNkhj5OYxSW2UjjJO4lxpM0gSdKYkTsEWZSVNGOzDgkrj0B4jTQO0oS9NY5T9V1d8BAYR5eETfyjIWQLgtc0z3K08C5KsxTwrcmT4sshSfL899kpisAAF1jxPEAH0faVAGg5XxAFNrErHxlVlQDwY5ADAlQBquSFQBjyMAFW8kRRNFMWAbE8UJYl0DJClgH4HoUwTalaUZRqIHhLqetRDEsR6HECSJUlyQQYAegYZQcMwJg+igY5ABezQAsTTMFa+vWzbhp2ml6SZWUwCAA)

实现`Trim<T>`，它是一个字符串类型，并返回一个新字符串，其中两端的空白符都已被删除。

例如

```typescript
type trimed = Trim<'  Hello World  '> // expected to be 'Hello World'
```

**正确解答**：结合上一题，易得 TrimRight 的实现方法，二者结合即可实现 Trim

```typescript
type Space = ' ' | '\n' | '\t'
type TrimLeft<S extends string> = S extends `${Space}${infer NewS}` ? TrimLeft<NewS> : S
type TrimRight<S extends string> = S extends `${infer NewS}${Space}` ? TrimLeft<NewS> : S
type Trim<S extends string> = TrimLeft<TrimRight<S>>
```

也可以用[第二种解法](https://www.typescriptlang.org/play?#code/PQKgUABBCMAMAcEC0EAqAnAlgW0spBheARgJ4QCCAdgC4AWA9leQGICuEAFAAICGtAMzYBKCAGJAtHKBJb3E0AptgAOAG17ykyzPPS9lePGMMRAGRmA7t31RAedqAG5wAGGHAB5UAPluAYf8DB2oHozQABygKjlAdW1AMm9AJjlAbx9AaPV3QDc9QBX4wD21AMAG0xDQ90A3RQlAEjlAe69AELdALy9AXzdgwF+EwCfdQGqIwAIlQBM0wCAGCwhAaPlAIM1m2y6aAGc8GlJFOQgaLGw5ABMIAF40MccAcigACTllZQYIAHUGdGUpiAWXCGBgCDkADyGAY3kpmk3iYYXV9c2dvYmFvC7bZuPABTqEAA4lo6GxiBBAFBygFPzQDQ7oAsf7oNBoih6AC5Tr1rnQAHQAKx6uN2AHNgHB4MAAF50JAAYQAcmAQMAwGzQBAAPrcnm8nkQQAG8vlAMdygEAPLl8yWciAstkDIYQADKil412GsyWSwAPocADpUbV6mjfeXDBzYRyK84XeRUCY9CA9UaYKgk46zK2XW32iC2AAkAG9laq5ABfQMugRydAQBlyADuitDtggOv9Acj0djCaTgeDauTEAA-HMnHHE8d0Ur2SAJVLeRBANK2gFXowAUri06-XuTLWThFLsaCNBsMAxAAKIARzYugANOOrnJbhBQxABOgGNhDtxTUgcbplHJXXIesA2DRMMoet8wKaINdeD1jzMIABtPBjhe3RyT6fKZzzBYnXQI450A0YjhcGd30-GhvynXR-ycJYgJAw4UJcSDoJuWCfwQ81FigQj0NA9DMKgD9sLg39EItMCYygVC6IgqDyJgqi8IAwioCArjDkgtDwIwlj50o3C-3wpYoH1XVBwEBhHl4GMZMYuSFOAoSsMXHD4PEgDGOYzSvzEmiCOkwd9I0gBdNka07LsIEAaDlfEAU2s7PrHswFAPBjkAMCVAGq5IVAGPIwAVbyRFE0UxYBsTxQliXQMkKWAfgenjaNqVpRlvIgeEQrC1EMSxHocQJIlSXJBBgB6BhlDPTAmD6KBjkAF7NACxNMw8oiwritisqaXpJlZTAIA)：

```typescript
type Space = ' ' | '\n' | '\t'
type Trim<S extends string> = S extends `${Space}${infer NewS}` | `${infer NewS}${Space}` ? Trim<NewS> : S
```

### 110・Capitalize

* [接受挑战](https://tsch.js.org/110/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCM0AwQLQQMIEMAOBLALmgNlgF4CmkSilV5ARgJ4QCCAdjgBYD2zDAYgK4QAFAAE0rAGZ8AlBADEgWjlAkt5ycJALYZ8aVYkKqATgXLlZpiIAyMwHduxqIDztQA3OEAAbpseQqQA8AFQB8TiEBg7UAwHUB1bUAyb0AmOUAQt0Aab0AAOUAqOVDAWetAG3jAI2NALjlAck1ATMVAGH-AN0VATXlUwF35QEBjQHzlQHYLQCAGGwhAaPlAIM0mp06cAGdyHDoMEggAY0xcAmISABMIAF5UMfdJzwByNhJ8fA4IAHcOfXwpld8IYGAIEgAPQeHVGZxtmiGVgAkNrd39w5XyTqcmk6ACnUIABxXBsPg0CCAKDlAKfmgGh3QBY-2wcDgMN0AFxnHrDNgAOgAVt08fsAObAWBwYBENiIFAAOTAIGAYFZoAgAH0udyedyIIADeWigGO5QCAHpzeRKORBmaz+oMIABZOiucYeEieADKF0uqmYU26EG6OH0WGYpJO8y1V11+ucABIAN6m8QkfQQHgAX0dztdEAASiQjR6AgB+e0OgCqGEG+lG3XVPF8XodAaDTgxEA1rLA7MlEoggGlbQCr0YAKV2a4rzfJlWA0+xwEDlQwdEAAogBHPgEAA0reuJFuEA9EHE+g4aggK2EjcQuII+BIZsDwD4OCw+G6PzAjZGaHjBvmAG1yC2+7dPO3O-hPEqVUsvCtxBwODQ0Ppjj2Vjwny+375fF3j1PHBzw7Ahr2VRYJnvHgAHkYIAIUYP13wnWCEKQ45-0Am5gIvMCb0gtVVkfR5XxQz8nwgH9MIAqATxwkDL3A28oPVFZyJo7D+1w0CrwItxWNWNByMYTi6KAxj8IggSiJWGhyPgsTewYvC+Ok1VlhWYZyJQJT6O4yS1JY2Sjn-CcABE9Ik1TmMIzSSHIlsrJU3jbJkzTxHInhnIMmz+I0+9SXIkEfLPPz1LvNi2HIl5Qp4pj-Mi1YsHIgBJOLDLcgK2IJciACkMvC4zNIAa3IgBpQrXMSwSVnwciABkqoSiLarUciFWaqTivvZhyPpLqjLs+8OHImDBqypKVgwciAAUJpq2S23IgBFBbWtk38P2Qv9aOU3zqo2zSNzMlYNXWnq2JwcjvAu4a2L4ciIzu9z7wAN3IgA1F7stWHZyIAdR+qbLnIgANYHarociAE1IdkohyIALU4gBdbMcxACtKylQBoOXiQBTa2xytpRZUByBOQAwJUAarlBUAY8jABVvZFUXRLFgBxfEiRJfRyUpYAxG6HZXWpWkGQpiAEUZ5m0UxbFulxQliTJCl4GAboOHwFcsC4XooBOQAXs0ALE0rGl1m5YVrnlZpOlGRlMAgA)

实现 `Capitalize<T>` 它将字符串的第一个字母转换为大写，其余字母保持原样。

例如

```typescript
type capitalized = Capitalize<'hello world'> // expected to be 'Hello world'
```

**正确解答**：还是通过模式匹配，使用内置类型 Uppercase 进行大写转换

```typescript
type MyCapitalize<S extends string> = S extends `${infer F}${infer Rest}` ? `${Uppercase<F>}${Rest}` : S
```

### 116・Replace ⭐

* [接受挑战](https://tsch.js.org/116/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCM0GwQLQQEoFMAOAbAhgYzUiURNKICMBPCAQQDsAXACwHs7qAxAVwgAoABHIwBmXAJQQAxIFo5QJLeUhmgC22HIsRYAlooBOOLESKTjEQBkZgO7dDUQHnagBucIAA3SqCAHgDKAGggcdLJd4AKiwAfA4QgGA6gOragGTegExyju7h0oAhboA03oAAcoBUcoAK2rEJDr7+4YD-ZoBGxoBcco7B4YBADFYQgNHygEGaDQ7tDADORAyUGGgQOpi4BAAmEAC8qMP4aK4A5L39nRA4QxCidACE897zm7sQ8zgA7mid-mjzIRDAwBCA+OaA2OaA9GZHS+er66fnlztE7QcDRugAp1CAAcW0TC45AggCg5QCn5oBod0AWP9MBgMDCdABcdy6eCYADoAFadQksHQAc2AsDgwAAXkxEABhAByYBAwDA3NAEAA+gLBULBRBAAbyKUAx3KAQA9+cK5XyIJzuR9pi45u4IGgAB6KOijFadBg6TR0SneIpKTU6tB6g1Gk1miDBK26-UQQ3G003KYa7WulYOAAkAG8TcI0DoIAAFIYAXxDFvjobo4cjUZYhtjQKgAH4fH5LX6bW75vMiLmIO5yxBsY4QzG0Engkn05nszXKzyQLL5UKIIBpW0Aq9GACldGj3ewLFVzNCoKQwICrgxAAKIARy4+m8y61-Tw89jGwLR34H0QBP0WBtlPOwC4DE0WE6ZbAdwXfQG86mzhGc32LBY5BrIBOiHPMwGgcI-7XGAKp4DgnSfFMADaRDbruDCuGuG5YK436zAskEAWsoHgXshHXGR-7kSEISeKhO5oHumHrvouEzG4f5ETopFHDxnEUUchGEeBNF0VAaGMRhWGsXhHHCUBxF7BBUG0YJ-7ASJtH0ehzHYWxaoEepCkgXsfECZxmliSuDFMdJOGyb+8ncYpvF6MpLDmU5lnaZJukyexv6gUFqmlqJYAALrcl244ThAgDQchkgCm1jFvZTi+4BQDcgBgSoA1XLioAx5GACreaIYliuLAPiRKkuSVI0vAwBCJ0Zw6AyTJskQNzIkVJWYjieKdASJJkhS1K0sAFxYHemhsN0mUQIAL2aAFiaFg9WV-WDdVI2tSy7JKmAQA)

实现 `Replace<S, From, To>` 将字符串 `S` 中的第一个子字符串 `From` 替换为 `To` 。

例如

```typescript
type replaced = Replace<'types are fun!', 'fun', 'awesome'> // 期望是 'types are awesome!'
```

**正确解答**：注意 From 为空的情况

```typescript
type Replace<S extends string, From extends string, To extends string> = S extends `${infer Pre}${From}${infer Post}`
  ? From extends ''
    ? S
    : `${Pre}${To}${Post}`
  : S
```

### 119・ReplaceAll ⭐⭐

* [接受挑战](https://tsch.js.org/119/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCM0JwQLQQEoFMAOAbAhgYzQEEstIlELKyAjATwkIDsAXACwHtH6AxAVwgAUAARwsAZrwCUEAMSBaOUCS3rOZoAtthwrEWAJYqATjlJQyMsxEAZGYDu3MmUB52oAbnCAAN0GgsSwAeAMoAaCG59dlUAgBV2AD5nCEAwHUAAOUAqOUB1bUAyb0AmORcfGLlAELdAASNASHNABW00zOcgkJjAf7NAI2NALjkXCOdAIAZbKEBo+UAgzXaXZ2dmAGcyZloMNAh9TFwCABMIAF5UafwiEi8AcmYIegwICcGNgI2II9ONyIhgYAhAfHNAbHNAejNT0fHDsn7nXsvACnUIAHE9KxeNQIIAoOUAp+aAaHdAFj-rGYzAwgwAXNchnhWAA6ABWg0x7H0AHNgLA4MAAF6sRAAYQAcmAQMAwMzQBAAPoczlczkQQAG8rlAMdygEAPdncsVsiCM5mvCZuGZrbw+fYADxUjFmgwgg2Y+h0jEJAUqqhVao1Wp1eoNEAiJrQ6s12t1+suSyVaFVdrNzgAJABvPViND6CAABSmAF8-UbI-7GIHgyH2Nrw18oAB+QLBY3u02ajYbMjpiA+QsQZEuP1htAxiIxuWrTxeRPaw1Z8JRFNkcslsCs8ViiCAaVtAKvRgApXDqi-s8qU6dQE7YyiC+iAAUQAjrwjAEV8rxnhtuGIGIs6chDLEBijFg7YS0INgLxmDosO8wIu8DhBnfFhAANpkHc92YLx103bx6w8dYNjEdh2GoHB9DODZ4MQ44YPYC40Ng9CLkiPwAN3NB9xAjcjC8CCFU2dCUKQ+DCSQnC8NOaiENw-CoEAojgNAsiKMbaDYJQmjjmE5jYMwsT2HQxi8IIoCSLA8iVkg7wth2CA9gOJDTmOCStjGO82LkriFN45TKIEuCENE-MsIwpjLKE1jIlkjjCOInjwPM-iUJwkTWLsvTpPElz2NXdzuNIrz3Aslj9DipC4NooKrPi1KjLc+TPKUmL+Jg6hYLSgqAtOArkoc-KCXy5zXPCrKopy+V+KQlqHKMgBdZkWRAScpwlQBoOXiQBTa16qdJSZUAyEuQAwJUAarl+UAY8jABVvOEESRVFgHRLFcXxIkSXgYBREGAB3IMKSpOkpogaFltWxEUTRQYMRxPECWJUlgEGdgsEfHROGGKBLkAF7NACxNaw7vWx7np2t7zppekpTAIA)

实现 `ReplaceAll<S, From, To>` 将一个字符串 `S` 中的所有子字符串 `From` 替换为 `To`。

例如

```typescript
type replaced = ReplaceAll<'t y p e s', ' ', ''> // 期望是 'types'
```

**正确解答**：在上题基础上，递归！

```typescript
type ReplaceAll<S extends string, From extends string, To extends string> = S extends `${infer Pre}${From}${infer Post}`
  ? From extends ''
    ? S
    : `${Pre}${To}${ReplaceAll<Post, From, To>}`
  : S
```

### 191・追加参数

* [接受挑战](https://tsch.js.org/191/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCMCc0QLQUL-xgCpUEPKgHU0kx+DcAjATwgFkBDAYwEsBTAKwgGVaBrAewCdKIAKAAIBbGg0YBnDj0oBKCAGJAtHKBJb0WVuAcwCuw+gDsALhNy4F5iIAyMwHdupqAD4IgRlcIgykYBm2iIG--QIvRdhCAedqADc6AAHKAVHKA2zaA0eoQAAYAggAOyQYAJolaugaGADwAYvoANBCJ9vGAMP+An9qAcXKAm36AWdqAIW6Av4pYgN4+cfFFVYCncoBTypGA33KA8IZdCYlVgCvxgHtqkYANpm1YCQDi8YBADPHrEICnRoCQ5gm9EM2AAkb72IBueoAU6oDU5oB8OuhdgFxyk-En2BuB8T+GJGkSajcWjJQy4P5pCBFCAAXgElAAXBB9LoiPRuKUiEiJIZgfpNPIYY4UcI0dxAhD6BAAEr0CTaAA2hlhZVSGSyOj0RkKJQgRE4nAZ9HcjlwwGAEEA+OaAbHNAPRm8KRJLJmOxuNo+NKAA8kfzBcL9ITiaj0bgfvFAo5ADTmgERjQAYRoBTc0AV4G1CAAbREYiYUi4vAAuvwABaGQzJCQI8WaWiGAPaIgAOmonGEwFEdC90l48muEAAIvQAG5x2icCCAKDlmq7AOGmgAOvf1BkNh8XpAtxwycFM0b0yYCUdL59zUejpRCUwHA0GIeia9F0CR0xAAR20dMMxf0iAALJvYABWaiyC0QbOrKMxohlwCn5oBod0AWP-10Ph4DGagBuOSOM8TTAODQYAALwDRAAGEADkwBAYAwDAUAIAAfXghDEIQiBAAN5ZpAGO5QBADzgpDcNgiAIKgylWTSfRMmyLl8mhKdDAyCQBDjRiNE0MMIHcEhDTY-QSFKcoWWozVaLI+j+EYuNmNY9UPHRMotAkTipJk6lcAAfgYpi5KRV0xI5CReN9TjlKgRUCxNaCQBwvDEIgQBpW0AVejAApXQBo+Usqz4IIyDaGEZIeGZYiAG8IAAUSXSgGVKILNTSahmQAXwgDxuCTCAAHJBEpRAXzCoV8TpYBtFXBkJBSoj-ipIDKDnBA4RSUjyM5XI8n4RFkWNDE+VVPECVhI1SXRTEBSFEUwGI2l6SZaqFVavr2qxCAcS6rUdUG-VOKVMziIqucACYWVq9kKMa-hOPzThaHSUptDI+gPHVId7BGsqaTpRlDF2uF+G1CArubW79CHE6zvSUrIWoSq6RZV1cEi6L8hC7QwryLb6GgUoxte6B7HsYpoai+gYryeHEeR7a0ZepltqxnGoHFVxjEnPGYsnbgkvJKB9rIjkcm5K72H0TgAHdeR+m67vSbGwF9KCYLc6zAGg5MJAFNrVy3I88zcEcQAwJUAark0MAY8jABVvO9gwfcVn1fd9P2-eAe30CQBfRf9ANAjWIGvQ3jYbR9zbfCQPy0a3fwkQUCrXEwHAgQAXs0ALE0bE902n0BC2-atgDgLAwiwCAA)

实现一个泛型 `AppendArgument<Fn, A>`，对于给定的函数类型 `Fn`，以及一个任意类型 `A`，返回一个新的函数 `G`。`G` 拥有 `Fn` 的所有参数并在末尾追加类型为 `A` 的参数。

```typescript
type Fn = (a: number, b: string) => number

type Result = AppendArgument<Fn, boolean>
// 期望是 (a: number, b: string, x: boolean) => number
```

**正确解答**：显而易见，本题 easy

```typescript
type AppendArgument<Fn extends (...args: any) => any, A> = Fn extends (...args: infer Args) => infer R
  ? (...args: [...Args, A]) => R
  : never
```

### 296・Permutation ⭐⭐⭐⭐

* [接受挑战](https://tsch.js.org/296/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBBMCcBsEC0EAKBTATgWwK4BcBDfASwHsA7SZJWu6gIwE8IA5Qs-MiASQGtcFbgAoAAgAdCFACZSyJTAEoIAYkC0coElvVYPJUo1FYYiAMjMB3btWqA87UANzoBUAwBAqgbx9A0eqAQt0AWioCTjQOhKgGH-AYDoOLoA28YBGxoAIRoACRoCQ5oD3yoC-AR4+gA6mgCN+rkHOgEAMFlAABgX4TOLoAM4Axpgk4vjURSUQJTgQALxoWHhEpJQAPADkAIJ9EAA+EH0AQsNjfQDCfQB8ANwQwMAQANqDfQA041N7c30AuqOb24fzh1OnY1sH40OXJ2f3u+NXjy93R4dP+99zp9Ju9tsdqAU8rkIAsIIAKdQgAHESPgABa4BgQQBQcoBT80A0O6ALH-Ufh8OJSgAuNb4CqogB0ACtSrSyJgAObAODwYAAL1RSFmrDAIGAYDAoAgAH0pdKZdKIIADeVcgGO5QCAHpLZRqJRBhaL6uh2jgCMRdD0ACp7ABKZXwrQgpthbQ2ptO6AAHvh0DJSpsKOgAG5YU4Afk2p3JkCtpRtbo9XogkZtIc25ogtLTGENXRNAFFXeUADa4aToM2W60LBbHcmhiCi8WajUQQDStoBV6MAFK6AaPl1Q25TqSNhxCybXqIABvCDZgCOuEI+b2uZK5RtAF8IAAzTBkbDjUR6pDlVGz-Oe1llYAEEj50p9XXFfXlQilMq2jbUBfoJc9Kcz-M9DOdY1em2BY9i2IZjgrHY31dRd8C-adZz-DojW6Ch+iGM4QUw+YQPOf4QWeW48NBYEbleAivkI8iHl+L4iK2YF8LIn5SNBcDIOg2D4J-JDM0AtCsJmDCZhw0CLgBKifnw1j6Io8SjlkmjGMBBi2NBZigXUtSIJAziPzg79EP-FCTQYMgyGPKRcI2NdZyfPZ8EwXB0HoxznL2WyrxcjioHfT9DN-Yys16X0A0waydKg8ExRAbsey1QBoOUAADlAFNrOKe21EVQGoWFADAlQBquUVQBjyMAFW8iRJMlKWAakDwZJkWXZTlgCkUoAHcsB5PkBRyiB8VK8rSQpKkaTq5k2Q5BBgFKCyL0oUoesAF7NACxNMwBsq4basZMb2V5flBR1MAgA)

实现联合类型的全排列，将联合类型转换成所有可能的全排列数组的联合类型。

```typescript
type perm = Permutation<'A' | 'B' | 'C'> // ['A', 'B', 'C'] | ['A', 'C', 'B'] | ['B', 'A', 'C'] | ['B', 'C', 'A'] | ['C', 'A', 'B'] | ['C', 'B', 'A']
```

**正确解答**：题目字越少，难度越大（x）

本题实现全排列，同时要利用联合类型的分散传参这个特性 [Distributive Conditional Types](https://www.typescriptlang.org/docs/handbook/2/conditional-types.html#distributive-conditional-types)

翻 issue 的时候翻到了这个优秀的解答：[TS 类型体操笔记 - 296 Permutation](https://juejin.cn/post/7165170011282079751)

`[T] extends [never]` 是由于 never 无法被准确判断，任何`extends never`的条件语句都会返回`never`，而我们需要返回的是空数组，在小册中的 [套路六：特殊特性要记清](https://juejin.cn/book/7047524421182947366/section/7048282437238915110) 有提到这一点。

```typescript
type Permutation<T, Rest = T> = [T] extends [never] ? [] : Rest extends Rest ? [T, ...Permutation<Exclude<T, Rest>>] : []
```

### 298・Length of String ⭐

* [接受挑战](https://tsch.js.org/298/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBBMCcAcEC0EAyBTAdgcwC4AsIB7AMwgGVcAnASx0mSSeYYCMBPCABRuwgDEAhjggAKAALYkABwA2w9AEoIAYkC0coElvVbnQBbOYJ1JZNHVUGyGDFTYiAMjMB3blaiBC6MDp3oHVtQGTegJjlAIW6A-qmAZXqAMP+A3j6APPKAcXIQAAaUtDgqslh4+LEQgEAMzhAAfBCAFOoQAOKm+ACurBCAUHKAp+aA0O6AWP-4uLjSAM4AXMDAuO0AxvgAdABW7UNEVNjAcPDAAF74SADCAHJgIMBgYKAQAPoHh0eHEIAG8n6Ax3KAgB77x3d7EJvbPRC47NLoaKkEAPIkCXRsAAecgQdAADx0mAAJu0IO1qID8gBeCgAbQA5CkcAQMQBdMBvD5fHH4P4AnAgsGQrCw+GInAAGggABVqVC6QjEtg0XiIKjeSiKOzaXDYgASADeXMBAF8pXQSOgqBAAEroBGy2IMAD8JLS5IZwPVCOZaJlTIgQ2tLLxuQYnVZmOxaXxzxAt3uRwggGlbQCr0YAKV0A0fKer0HR5bGj6Sa4V7vT6SiAAUQAjuULMyk+CPv1Y7KICQqERdBAMeIiegkIMLC6NcByrgaLJ2hjthWIP1BO0NfyIGiGFmc7ggan07IgRhSYbuUCMRjcsyAAy5BcD7PoXMjtMWCffMn-I2zgDW5V0NCPRHnzIAbCvGWuh1ux7upweZxiqOg6IIrxAAKx3g+G7DqOO6Tgab6ArO5BEOUMIAITJuU0j4EQmA0Kev4AIy3quBI7B6YbeoA0HKAABygCm1qGYYRgRDD5IAYEqANVy5yAMeRgAq3s0rQdN0vQDMMYwTFMMwIMAwjtAA7sqCxLGsdEQA07GcW0XQ9H0gyjOMkzTLMwDtEQsgNjQaHtHJgAvZoAWJqOEp3GqXxGmCdMiwrOsTxgEAA)

计算字符串的长度，类似于 `String#length` 。

**正确解答**：不讲武德版当然就是 `type LengthOfString<S extends string> = S['length']` 当然，讲武德版就是这样 ⬇️

```typescript
type LengthOfString<S extends string, T extends string[] = []> = S extends `${string}${infer Rest}`
  ? LengthOfString<Rest, [string, ...T]>
  : T['length']
```

### 459・Flatten ⭐⭐⭐

* [接受挑战](https://tsch.js.org/459/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBAsCsCcEC0EBiAbAhgF2wUwDtJklSziAjATwgC8ALAewFcqBLAWzYIHMIAKAAIBjehQBOjAJQQAxIFo5QJLeczOPGYqxYrJ0RAGRmA7ty1RAFOqBN+MBUcoERjQBhG8wDD-gA3lAAOmBAyMCZioAA5C4FLjQOvKgA6mgCN+gCFugN4+gNHq9oBueoAocoAr8YB7aoCCRoDOeoBoyiHBkYBADMYQgNHygEGaAFz5AAaV2ADOxNhUAA54EABmWLiEEAC8aO34BAA8ANoAjAA0EABME0MAzBPQALozQ0OwixuLAHwQwMAQoxPTEPMwE+vEleX5OyYQAOJs2PTMFBCAUHKAp+aA0O6AWP-0uAa1RKexqogAdAArargxjiHjAODwYAMJAAYQAcmAQMAwGBQBAAPrEkmkkkQRwhQDHcoBADyJZIZhIgOLx9SavRw-QGAEE1BA8AAPfoAE2qEEwBCoQ223QgvPE-KFhFFB24LTwCoAkvgOBNwfq1RqIAAlPDVbCLYgAfgO+vB-G1eA4ipFYolUsWEBtGE5hAGjo4OxKBwDiykev1Po6g1N5q2lqgweleIJjIZEEA0raAVejABSuBXpafJLM4DTh2AgbOaAG8IABRACOzEw6AmtYFTWE5YAvq1JM6AOSCStIUTN9CEHhm4DMbBsdDVfusxrNYSYapm2VDYhtjvYAYNpvoAZRrnSrYzbbn7ftvCd-eN5vHvp+w5TCanJbng7jN8nBaXsZr13e9DyfX1BlfIZJg2L9X2grYrygHdbz3A9HxPF8f2OOZ-xWNZNm2GYsPfBZzgAoCUJA9DnwgmsWkYRhg37ChVH7ABuKZgxGAAGCAuwmft6MYFjxH7QiDjohimJE9jOIgHi+IEoSZPIy18RAAtCyZQBoOU8QBTa00wtmVxUBiB2QAwJUAarlKUAY8jABVvf5AWBUFqghaFYXhREEGACVqgAdw1FF6HRLEoB2H57Mc7AgRBYAwXoKEYThBEkWAapGHQGc2EYAhajCiBABezQAsTUMKKYpctyks81FMWxXEwCAA)

在这个挑战中，你需要写一个接受数组的类型，并且返回扁平化的数组类型。

例如:

```typescript
type flatten = Flatten<[1, 2, [3, 4], [[[5]]]]> // [1, 2, 3, 4, 5]
```

**正确解答**：经典的数组拍平，需要注意的是...展开需在外层，`Item extends any[] ? ...Flatten<Item> : Item` 是不行的......

```typescript
type Flatten<Arr extends any[]> = Arr extends [infer Item, ...infer Rest]
  ? [...(Item extends any[] ? Flatten<Item> : [Item]), ...Flatten<Rest>]
  : []
```

### 527・Append to object ⭐

* [接受挑战](https://tsch.js.org/527/play/zh-CN)
* [我的解答](https://www.typescriptlang.org/play?#code/PQKgUABBCsBMDsEC0ECCAHdBTAdgEwgBcB7CYgIwCssBjQyZJJ5h8gTzXwCcsOBpLgEMAzsQBuwgNYcAFAAFyPAMwAGSUIBsAThrCAlBADEgWjlAkt5GK1Okkm9hDBoacRAGRmA7twdRAedqAG50AAcoBUcoBccoClxoDHyoDftoAFSoGADaaA6tqArdaAIW6A3j6A0eqAQAyAp9EZIYBspoCQcgGAQ8qADqaAMP+AK-GAe2qAZHqAkOYJKeEZmZ4QgNHygEGaAFwdAAZDhPZQhGzYEAAqWMKEEAC8EADeEACWeL0QAOQAjNsQAL4M45MASrMArgA280sY2PhTxADyVLSEADwzcwA0O2JBNdLlhtv8ACwAPggwGAECwAA9sHQsAQSBByFgVutNjt9v9AcCsFtwUcGEMBh1oYAKdQgAHE1oQABaXcgQQBQcoBT80A0O6ALH+mYRCOhhL1YSMaEyAHSUYSS4hcADmwDg8GAAC8mUgAMIAOTAIGAYCNoAgAH1zRbLRaIIADeWSgGO5QCAHmara7TRADUbTliHrg8M83lYvlN4QjCH7hBALjR5XhPnMuGscAr-oIcGxIf8AKqh8P4SMJpMpiAANWhS2WDAA2nxeOscBBbGxiAAzaYAXS2UxrvHbYEOEAAZCtq036xAs53S-3cxH6y2sFwIIGGAB+bE18dN1vLqhTwM19tkqBbHBYMSL40gF1uy0QQDStoBV6MAFK6dG+380ew1rAC26Hl8zetiACiACOlxAv8wFIh8RwQC2XDED+OxyN6SASkC1y4AqszAJchBrNcwjbF6ExYuGcy7IsI5QE2WzbDQgiECRUCEiC9EKjwuAkccYBARRhDQcihBURWDB0TsjHMQwbHEjsnFYNxDBMkhcnkMQxBYWm-akZMAmwNRla0bw9F4MQCoHAAPhAlz4FgLZJqiMlAuxOwAO5MoyoIMMItlbIQXAgjpfFkUQsyCTBdAGWJxlsKZ5lWTZdkOWeeDOUS9EeV5LEQL5OD+YFWDKapWy7MF-HhUohniSZknEG5OWyfRbBYNc1z1TleVbC2QLCEVvEVXMQkfFVMWNrVDEdelrnbC1bVTVAXXwb1RVQGswgALLEMyi5nJcwjCGsgjdStEDWbZeD2Y5aUDaFjF9ZGSxVgww10J8YEQdcny+k8rzvG9Am7P82wqT+oL-OpmlYGmmZhUNkUiZCmYvQj73gUC32YH6Ab-V8+nA6D4MQLssMCa9hCwEjvwo8JaOfZjjz+n9QafAJSjA+tW07Vwe0HUdYLLURWLncl12k+F5NKFTYB9kaYAmh+d6ANByfiAKbW74fl+8vgFA0KAGBKgDVcnagDHkYAKt78oKwqisA4pSjKcqKsqCDAGmwhuYu6qarqDDQjyZsW0KIpisIErSrK8pKiqwCiMCBHEDgowQNCgAvZoAWJruAHVvB6H9sR572p6p6YBAA)
* 实现一个为接口添加一个新字段的类型。该类型接收三个参数，返回带有新字段的接口类型。

例如:

```typescript
type Test = { id: '1' }
type Result = AppendToObject<Test, 'value', 4> // expected to be { id: '1', value: 4 }
```

**正确解答**：先将交叉类型整出来，再把交叉类型遍历一遍。

```typescript
type AppendToObject<T extends Record<string, any>, U extends string, V> = {
  [Key in keyof T]: T[Key]
} & {
  [key in U]: V
} extends infer Obj
  ? { [K in keyof Obj]: Obj[K] }
  : never
```

看到一种很有趣的 [解法](https://github.com/type-challenges/type-challenges/issues/536)

```typescript
type AppendToObject<T, U extends keyof any, V> = {
  [K in keyof T | U]: K extends keyof T ? T[K] : V
}
```