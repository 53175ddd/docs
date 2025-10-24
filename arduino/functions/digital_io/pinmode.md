# `pinMode()`

<!-- 説明 -->

## 説明

第一引数で指定したピンが入力として動作するか，出力として動作するかを第二引数で設定します．  
`INPUT_PULLUP` を指定すると，内蔵プルアップ抵抗を有効にできます．内蔵プルダウン抵抗を持つ一部のコントローラでは，`INPUT_PULLDOWN` を指定することができます．

<!-- 構文 -->

## 構文

`pinMode(pin, mode)`

`pin` : 操作したいピンの番号; `D10` の場合は `10` など．  
`mode` : 設定したい状態; `INPUT`, `OUTPUT`, `INPUT_PULLUP` (, `INPUT_PULLDOWN`)

<!-- コード例 -->

## コード例

以下の例では，`4` 番ピンを入力に，`5` 番ピンを出力に，`6` 番ピンを入力にしつつ内蔵プルアップ抵抗を有効にしています．

```cpp
void setup() {
  pinMode(4,  INPUT);
  pinMode(5, OUTPUT);
  pinMode(6,  INPUT_PULLUP);
}

void loop() {
}
```

<!-- 関連 -->

## 関連

- [digitaiRead()](./digitalread.html)
- [digitaiWrite()](./digitalwrite.html)
