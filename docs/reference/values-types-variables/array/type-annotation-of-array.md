---
sidebar_label: 配列の型注釈
---

# 配列の型注釈 (type annotation)

TypeScriptでは、配列に型注釈する方法が2通りあります。

## Type\[]

1つ目の型注釈は、要素の型の後ろに`[]`をつける書き方です。たとえば、数値型の配列の型注釈は`number[]`と書きます。

```ts twoslash
let array: number[];
array = [1, 2, 3];
```

## Array&lt;T>

2つ目の型注釈は、`Array<T>`を用いる書き方です。`T`には要素の型を書きます。たとえば、数値型の配列の型注釈は`Array<number>`と書きます。

```ts twoslash
let array: Array<number>;
array = [1, 2, 3];
```

## Type\[]とArray&lt;T>どちらを使うべきか？

TypeScriptでの配列の型注釈は、`Type[]`と`Array<T>`の2通りあるわけですが、その違いは書き方だけです。コード上の意味、つまり、コンパイラのチェックの内容はどちらも同じです。したがって、どちらの書き方を選ぶかは、書き手の好みになります。ただし、プロジェクトとしてはどちらの書き方にするかは統一しておくべきです。
