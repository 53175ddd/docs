# `digitalRead()`

<!-- 説明 -->

## 説明

引数で指定したピンの状態を読み取り，`HIGH` か `LOW` を返します．

<!-- 構文 -->

## 構文

`digitalRead(pin)`

`pin` : 状態を読み取りたいピンの番号; `D10` の場合は `10` など．

`int` 型などの整数型で宣言された変数を使うことで，読み取った情報を保存し，使うことができます．

<!-- コード例 -->

## コード例

以下の例では，`5` 番ピンを入力に設定し，`int` 型で宣言した変数 `status` に `5` 番ピンの状態を格納しています．

```cpp
const int input_pin = 5;

void setup() {
  pinMode(input_pin,  INPUT);

  int status;
  status = digitalRead(input_pin);
}

void loop() {
}
```

<!-- 関連 -->

## 関連

- [pinMode()](./pinmode.html)
- [digitaiWrite()](./digitalwrite.html)
