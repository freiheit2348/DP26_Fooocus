<div align=center>
<img width="3335" height="2000" alt="image" src="https://github.com/user-attachments/assets/54bd65b0-6f3e-424d-a977-f012aa53fa8c" />

</div>

# BUNKA VF DP26 — DAY2 Fooocus ローカル起動用リポジトリ

> **このリポジトリは [lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus) のフォークです。**  

---

## 🌐 DAY1（Google Colab）との違い

| | DAY1 : Google Colab | DAY2 : ローカル起動 |
|---|---|---|
| 実行場所 | クラウド上の他人のPC | **自分のPC** |
| GPU | Googleが用意したGPU | **自分のGPU** |
| ネット接続 | 必要（常時） | 起動後は不要 |
| 無料枠の制限 | あり（時間制限など） | **なし** |
| 速度 | Googleのサーバー次第 | **自分のPCスペック次第** |
| データの保存 | セッション終了で消える場合あり | **ローカルに永続保存** |

DAY1 では Google Colab を通して、世界のどこかにある Google のサーバー上のPCの性能を借りて Fooocus を実行していました。便利な反面、無料枠には利用時間の制限があり、セッションが切れると作業が中断されることもあります。

**DAY2 では自分のPC上で直接 Fooocus を動かします。** 自分のマシンなのでいつでも・何時間でも使え、生成した画像もそのままローカルに保存されます。GPU を積んだPCであれば生成速度も出やすく、より快適に画像生成を楽しめます。

---

## ⬇️ ダウンロード（Windows）
<div align="center">
### 1. ダウンロード先はCドライブの中へ配置します。
### **[📦 Fooocus for Windows — ここからダウンロード](https://github.com/lllyasviel/Fooocus/releases/download/release/Fooocus_win64_2-1-831.7z)**

（ファイルサイズ：約 1.8GB　形式：`.7z`）

</div>

> **💡 補足**  
> 起動時に自動アップデートが走るので、ダウンロードするファイルは上記の古いバージョンのままで OK です。

---

## ◉起動手順

### 1. ダウンロードしたファイルを解凍する
### --🌟DAY2の事前準備としてこの解凍までを完了させてください

以降
### 2. `run.bat` をダブルクリック

解凍したフォルダの中にある `run.bat` をダブルクリックします。  
黒いターミナル画面が出てきますが、**そのまま閉じずに待ちます**。

### 3. ブラウザが自動で開く

しばらく待つと、ブラウザが自動で開き Fooocus の画面が表示されます。  
（表示されない場合は、ターミナルに表示されている `http://127.0.0.1:7865` などのURLをコピーしてブラウザのアドレスバーに貼り付けてください）

### 4. プロンプトを入力して画像生成！

テキストボックスにプロンプト（生成したい画像の説明）を英語で入力して「Generate」ボタンを押すだけです。

---

## 💻 動作環境（最低要件）

| 項目 | 必要スペック |
|---|---|
| OS | Windows 10 / 11 |
| GPU | NVIDIA（VRAM 4GB 以上） |
| ストレージ空き容量 | 20GB 以上推奨 |
---

## ❓ うまく起動しない場合

- **`run.bat` を実行してもブラウザが開かない** → ターミナルのURLを手動でブラウザに貼り付けてみてください
- **生成がとても遅い** → GPU が認識されていない可能性があります。NVIDIAドライバーを最新にしてみてください

---

## 🔗 オリジナルリポジトリ

本リポジトリは以下のリポジトリをフォークしたものです。
- [lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus)

Note that if no `--language` is given and at the same time `Fooocus/language/default.json` exists, Fooocus will always load `Fooocus/language/default.json` for translation. By default, the file `Fooocus/language/default.json` does not exist.
