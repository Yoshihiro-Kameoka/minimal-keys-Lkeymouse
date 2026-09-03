# minimal-keys-Lkeymouse

[minimal-keys](https://github.com/hyhy-masa/minimal-keys-release) 向け ZMK ユーザー設定。  
roBaish / Cygnus と同じキー配列・レイヤー・ポインティング方針を、minimal-keys の配列に合わせて移植しています。

## ハードウェア

- ベース: [hyhy-masa/minimal-keys-release](https://github.com/hyhy-masa/minimal-keys-release)
- トラックボール付き右半分（badjeff PMW3610 + input processors）
- エンコーダは **左手**（最上段右端付近）。クリックキーはエンコーダ直下の **MB1 / MB2** を維持

## roBaish からの主な設定

| 項目 | 値 |
|---|---|
| エンコーダ | `steps=34`, `triggers=24`, `SCRL_VAL=63`, `tap-ms=30`, listener なし |
| ベース層スクロール | 縦（`SCRL_UP` / `SCRL_DOWN`） |
| マウス層スクロール | 横（`SCRL_LEFT` / `SCRL_RIGHT`） |
| トラックボール CPI | 800, `force-awake` |
| ボールスクロール | レイヤ 6/7, `zip_scroll_scaler 1 30` |
| BLE 間隔 | MIN=6, MAX=12 |

## ビルド

GitHub Actions で `minimal-keys`（右）/ 左 / settings_reset が生成されます。

## 注意

- [hyhy-masa/minimal-keys-farmware](https://github.com/hyhy-masa/minimal-keys-farmware) の G-plan 専用ドライバ版とは **別リポ** です（こちらは roBaish 系 badjeff スタック）。
- 初回やレイヤ構造変更後は左右とも焼き直してください。
