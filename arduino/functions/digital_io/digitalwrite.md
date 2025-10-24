# `digitalWrire()`

<!-- 説明 -->

## 説明

第一引数で指定したピンから第二引数で指定した状態を出力します．  
`LOW` を指定した場合は GND と同じ電圧（0V）を，`HIGH` を指定した場合は 5V または 3.3V を出力します．このときの電圧はボードによって異なり，多くはコントローラの電源電圧です．

ピンが `pinMode()` 関数によって `INPUT` に設定されている状態で `digitaiWrite()` を実行すると，そのピンの内蔵プルアップ抵抗を操作します．`HIGH` で有効に，`LOW` で無効になります．  
ただし，内蔵プルアップの操作を操作するには，`pinMode()` 関数を使用することが推奨されます．

<!-- 構文 -->

## 構文

`digitalWrite(pin, value)`

`pin` : 操作したいピンの番号; `D10` の場合は `10` など．  
`value` : `HIGH` または `LOW`

<!-- コード例 -->

## コード例

以下の例では，`4` 番ピンを出力にした後，`HIGH` を出力するようにしています．

```cpp
const int output_pin = 4;

void setup() {
  pinMode(output_pin, OUTPUT);
  digitalWrite(output_pin, HIGH);
}

void loop() {
}
```

<!-- 関連 -->

## 関連

- [pinMode()](./pinmode.html)
- [digitaiRead()](./digitalread.html)
