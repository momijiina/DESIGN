# Google デザインシステム

## 1. 概要・世界観

Googleのデザインは「情報への最短距離」を体現する。装飾を徹底的に排除し、コンテンツとアクションを最前面に置くクリーンで機能的なインターフェース。Material Design 3（M3）の設計言語に基づき、サーフェス・エレベーション・モーションの3要素で視覚的階層を構築する。

カラーシステムはGoogle Blueを基調としつつ、Googleの4色ブランドカラー（ブルー・レッド・イエロー・グリーン）がプロダクトアイデンティティとして機能する。ただしUI上では**Google Blue（`#1a73e8`）が圧倒的に支配的**で、他の3色はロゴ・イラスト・ステータスインジケーターに限定される。白い広大なキャンバスに、ブルーのアクセントと`Google Sans`の丸みのあるジオメトリックタイポグラフィが乗る——それがGoogleの視覚的シグネチャー。

アイコンシステムには**Material Design Icons**（`Material Symbols`）を全面採用。`material-symbols-outlined`（アウトライン）、`material-symbols-rounded`（ラウンデッド）、`material-symbols-sharp`（シャープ）の3バリアントがあり、Googleのプロダクトでは主に**Outlined**と**Rounded**を使用する。バリアブルフォントとして提供され、`FILL`（塗り 0/1）、`wght`（ウェイト 100–700）、`GRAD`（グレード -25〜200）、`opsz`（オプティカルサイズ 20–48）の4軸で精密に制御可能。

**主な特徴:**
- Google Sans（ディスプレイ/見出し）＋ Roboto（本文/UI）の2フォントシステム
- Google Blue（`#1a73e8`）が唯一のプライマリアクションカラー
- Material Design Icons（Material Symbols）による統一アイコンシステム
- 白キャンバス＋最小シャドウ＋大量の余白——「Googleの白さ」
- 角丸はフルピル（999px）CTAと8px標準コンテナの二極
- エレベーションはトーナルサーフェス（色調シフト）とシャドウの併用
- 8pxグリッドベースの厳格なスペーシング
- アクセシビリティファースト——WCAG AA以上を全要素で担保

## 2. カラーパレットと役割

### プライマリ
| 名前 | 色コード | 用途 |
|------|----------|------|
| Google Blue | `#1a73e8` | プライマリCTA、リンク、選択状態、フォーカス。UIの唯一のアクションカラー |
| Google Blue Hover | `#1765cc` | ボタンホバー |
| Google Blue Active | `#1b66c9` | ボタンactive/pressed |
| Pure White | `#ffffff` | プライマリキャンバス、カードサーフェス |
| Near Black | `#202124` | プライマリテキスト、見出し |

### ブランド4色（限定使用）
| 名前 | 色コード | 用途 |
|------|----------|------|
| Google Blue | `#4285f4` | ロゴ、ブランドイラスト（UIアクションには`#1a73e8`を使用） |
| Google Red | `#ea4335` | ロゴ、エラー状態、破壊的アクション |
| Google Yellow | `#fbbc04` | ロゴ、警告状態、スター/レーティング |
| Google Green | `#34a853` | ロゴ、成功状態、完了インジケーター |

### サーフェスと背景
| 名前 | 色コード | 用途 |
|------|----------|------|
| キャンバスホワイト | `#ffffff` | プライマリ背景 |
| サーフェスグレー | `#f8f9fa` | セカンダリサーフェス、セクション交互背景 |
| サーフェスダーク | `#f1f3f4` | カードホバー背景、入力フィールド背景 |
| ディバイダー | `#dadce0` | ボーダー、ディバイダー、セパレーター |
| オーバーレイ | `rgba(0,0,0,0.6)` | モーダルスクリム |

### テキストスケール
| 名前 | 色コード | 用途 |
|------|----------|------|
| プライマリ | `#202124` | 見出し、本文（ニアブラック） |
| セカンダリ | `#5f6368` | 説明文、メタデータ、プレースホルダー |
| ターシャリ | `#80868b` | 無効テキスト、ヒント |
| インバース | `#ffffff` | ダーク/ブルーサーフェス上テキスト |
| リンク | `#1a73e8` | インラインリンク——ホバーで下線 |

### ステータス
| 名前 | 色コード | 用途 |
|------|----------|------|
| エラー | `#d93025` | エラーメッセージ、バリデーション |
| エラー背景 | `#fce8e6` | エラーフィールドのソフト背景 |
| 成功 | `#1e8e3e` | 成功メッセージ、完了 |
| 成功背景 | `#e6f4ea` | 成功フィールドのソフト背景 |
| 警告 | `#f9ab00` | 警告メッセージ |
| 警告背景 | `#fef7e0` | 警告フィールドのソフト背景 |
| 情報 | `#1a73e8` | 情報メッセージ（プライマリブルーと同一） |
| 情報背景 | `#e8f0fe` | 情報フィールドのソフト背景 |

## 3. タイポグラフィ

### フォントファミリー
- **ディスプレイ/見出し**: `Google Sans`, `Noto Sans JP`, `Roboto`, `Arial`, `sans-serif`
- **本文/UI**: `Roboto`, `Noto Sans JP`, `Arial`, `sans-serif`
- **モノスペース**: `Roboto Mono`, `monospace`
- **アイコン**: `Material Symbols Outlined`, `Material Symbols Rounded`

### タイプスケール

| 役割 | フォント | サイズ | ウェイト | 行間 | 字間 | 備考 |
|------|----------|--------|----------|------|------|------|
| ディスプレイL | Google Sans | 57px (3.56rem) | 400 | 1.12 | -0.25px | ランディングページヒーロー |
| ディスプレイM | Google Sans | 45px (2.81rem) | 400 | 1.16 | 0px | セカンダリヒーロー |
| ディスプレイS | Google Sans | 36px (2.25rem) | 400 | 1.22 | 0px | フィーチャーセクション |
| ヘッドラインL | Google Sans | 32px (2rem) | 400 | 1.25 | 0px | ページセクション見出し |
| ヘッドラインM | Google Sans | 28px (1.75rem) | 400 | 1.29 | 0px | サブセクション見出し |
| ヘッドラインS | Google Sans | 24px (1.5rem) | 400 | 1.33 | 0px | カード見出し |
| タイトルL | Google Sans | 22px (1.38rem) | 500 | 1.27 | 0px | モジュールタイトル |
| タイトルM | Google Sans | 16px (1rem) | 500 | 1.50 | 0.15px | コンポーネントタイトル |
| タイトルS | Google Sans | 14px (0.88rem) | 500 | 1.43 | 0.1px | 小タイトル |
| ボディL | Roboto | 16px (1rem) | 400 | 1.50 | 0.5px | 標準本文 |
| ボディM | Roboto | 14px (0.88rem) | 400 | 1.43 | 0.25px | コンパクト本文 |
| ボディS | Roboto | 12px (0.75rem) | 400 | 1.33 | 0.4px | 補足テキスト |
| ラベルL | Roboto | 14px (0.88rem) | 500 | 1.43 | 0.1px | ボタンラベル、ナビ |
| ラベルM | Roboto | 12px (0.75rem) | 500 | 1.33 | 0.5px | バッジ、タグ |
| ラベルS | Roboto | 11px (0.69rem) | 500 | 1.45 | 0.5px | マイクロラベル |

### タイポグラフィの原則
- **2フォントの明確な分業**: Google Sansはディスプレイ〜タイトルの「声」、Robotoは本文〜ラベルの「読む」テキスト。混用しない
- **ウェイトの節制**: Google Sansは400（ディスプレイ/見出し）と500（タイトル）の2ウェイトのみ。Robotoは400と500。700はほぼ使わない——Googleは太字で叫ばない
- **字間の微調整**: サイズが小さくなるほど字間が広がる（ディスプレイ-0.25px → ラベル0.5px）。M3のスケーリング原則に準拠
- **行間の一貫性**: 1.12（ディスプレイ）→ 1.50（ボディ）のスムーズなグラデーション

## 4. コンポーネント

### アイコンシステム

Googleのアイコンには**2つの導入方法**がある。新規プロジェクトでは**Material Symbols**（バリアブルフォント版）を推奨するが、既存プロジェクトや軽量導入では**Material Design Icons**（旧版・固定ウェイト）も引き続き利用可能。

---

#### A. Material Symbols（推奨・新世代）

バリアブルフォントとして提供。FILL/wght/GRAD/opszの4軸で動的に制御できる。

**導入方法**
```html
<!-- Google Fonts経由 -->
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />

<!-- Rounded バリアント -->
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Rounded:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
```

**使用方法**
```html
<span class="material-symbols-outlined">search</span>
<span class="material-symbols-rounded">home</span>
```

**バリアブルフォント軸**
| 軸 | 範囲 | デフォルト | 用途 |
|----|------|-----------|------|
| FILL | 0–1 | 0 | 0=アウトライン、1=塗りつぶし。選択/アクティブ状態で1に |
| wght | 100–700 | 400 | アイコンの太さ。周囲テキストのウェイトに合わせる |
| GRAD | -25〜200 | 0 | グレード。ダーク背景では正値で視認性向上 |
| opsz | 20–48 | 24 | オプティカルサイズ。アイコンサイズに合わせて設定 |

**サイズスケール**
| サイズ | px | opsz | 用途 |
|--------|-----|------|------|
| 極小 | 18px | 20 | インラインテキスト、メタデータ |
| 小 | 20px | 20 | ボタン内、コンパクトUI |
| 標準 | 24px | 24 | ナビ、リスト、一般UI |
| 中 | 36px | 36 | フィーチャーアイコン |
| 大 | 48px | 48 | ヒーロー、空状態イラスト |

---

#### B. Material Design Icons（旧版・軽量導入）

固定ウェイトのアイコンフォント。バリアブル軸は持たないが、導入が簡単で軽量。npm パッケージ `material-design-icons` としても配布。

**導入方法**
```html
<!-- Google Fonts経由（最もシンプル） -->
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />

<!-- バリアント別 -->
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons+Outlined" />
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons+Round" />
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons+Sharp" />
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons+Two+Tone" />

<!-- npm経由 -->
<!-- npm install material-design-icons -->
<!-- node_modules/material-design-icons/iconfont/material-icons.css を参照 -->
```

**使用方法**
```html
<!-- Filled（デフォルト） -->
<span class="material-icons">search</span>
<span class="material-icons">home</span>
<span class="material-icons">favorite</span>

<!-- Outlined -->
<span class="material-icons-outlined">search</span>

<!-- Rounded -->
<span class="material-icons-round">home</span>

<!-- Sharp -->
<span class="material-icons-sharp">settings</span>

<!-- Two Tone -->
<span class="material-icons-two-tone">info</span>
```

**5つのバリアント**
| クラス名 | スタイル | 用途 |
|----------|----------|------|
| `material-icons` | Filled（塗りつぶし） | デフォルト、選択/アクティブ状態 |
| `material-icons-outlined` | Outlined（アウトライン） | 非選択状態、一般UI |
| `material-icons-round` | Rounded（角丸） | フレンドリー、コンシューマー向け |
| `material-icons-sharp` | Sharp（シャープ角） | テクニカル、エッジの効いたUI |
| `material-icons-two-tone` | Two Tone（2トーン） | 装飾的、フィーチャーアイコン |

**サイズ制御**
```css
/* デフォルト24px。CSSでサイズ変更 */
.material-icons { font-size: 24px; }
.material-icons.md-18 { font-size: 18px; }
.material-icons.md-36 { font-size: 36px; }
.material-icons.md-48 { font-size: 48px; }

/* 色はcolor プロパティで制御 */
.material-icons { color: #5f6368; }
.material-icons.active { color: #1a73e8; }
```

---

#### Material Symbols vs Material Design Icons 比較

| 項目 | Material Symbols（新） | Material Design Icons（旧） |
|------|----------------------|---------------------------|
| 提供方式 | バリアブルフォント | 固定ウェイトフォント |
| カスタマイズ | FILL/wght/GRAD/opszの4軸 | CSSのfont-size/colorのみ |
| バリアント | Outlined / Rounded / Sharp | Filled / Outlined / Rounded / Sharp / Two Tone |
| アイコン数 | 2,500+（継続追加） | 約2,000（更新停止） |
| npm | `@material-symbols/font-*` | `material-design-icons` |
| 推奨用途 | 新規プロジェクト、M3準拠 | 既存プロジェクト、軽量導入、レガシー対応 |

**選択指針**: 新規開発ではMaterial Symbolsを使用。既存プロジェクトでMaterial Design Iconsを使用中なら無理に移行する必要はないが、新しいアイコンが必要な場合はMaterial Symbolsの併用を検討。

---

#### 共通の使い分けルール
- **Outlined / アウトライン（デフォルト）**: 非選択状態、一般UI、ナビゲーション
- **Filled / 塗りつぶし**: 選択/アクティブ状態（例: ナビの現在ページ、お気に入り済み）
- **Rounded / 角丸**: よりフレンドリーな文脈（コンシューマー向け、カジュアルUI）
- ボタン内アイコン: テキストの左に8pxギャップで配置、サイズ18–20px
- アイコン色: 通常`#5f6368`（セカンダリテキスト）、アクティブ時`#1a73e8`（Google Blue）

### ボタン

**Filled（プライマリ）**
- 背景: `#1a73e8`（Google Blue）
- テキスト: `#ffffff`、Roboto 14px / 500 / 字間0.1px
- パディング: 10px 24px
- 角丸: 999px（フルピル）——M3のFilledボタンシグネチャー
- ホバー: `#1765cc`＋シャドウ `0 1px 3px rgba(0,0,0,0.3)`
- アクティブ: `#1b66c9`
- フォーカス: `2px solid #1a73e8` アウトライン（2pxオフセット）
- アイコン付き: 左にMaterial Symbol 18px、テキストとの間に8pxギャップ

**Outlined（セカンダリ）**
- 背景: transparent
- テキスト: `#1a73e8`
- ボーダー: `1px solid #dadce0`
- 角丸: 999px
- ホバー: 背景`#e8f0fe`（ブルーティント）
- アクティブ: 背景`#d2e3fc`

**Tonal（ターシャリ）**
- 背景: `#e8f0fe`（ソフトブルー）
- テキスト: `#1a73e8`
- 角丸: 999px
- ホバー: 背景 やや暗く
- アクション重要度: Filled > Tonal > Outlined > Text

**Text（最小強調）**
- 背景: transparent
- テキスト: `#1a73e8`
- パディング: 10px 12px
- ホバー: 背景`rgba(26,115,232,0.08)`

**FAB（フローティングアクションボタン）**
- 背景: `#ffffff` or `#e8f0fe`
- アイコン: `#1a73e8`、Material Symbol 24px
- 角丸: 16px（小FAB）、28px（標準FAB）
- シャドウ: `0 2px 6px rgba(0,0,0,0.15), 0 1px 2px rgba(0,0,0,0.3)`
- ホバー: シャドウ強化＋エレベーション上昇

### カードとコンテナ

**Elevated Card**
- 背景: `#ffffff`
- 角丸: 12px
- シャドウ: `0 1px 2px rgba(0,0,0,0.3), 0 1px 3px 1px rgba(0,0,0,0.15)`
- ホバー: シャドウ強化
- パディング: 16px

**Filled Card**
- 背景: `#f8f9fa`（サーフェスグレー）
- 角丸: 12px
- シャドウ: なし
- ボーダー: なし

**Outlined Card**
- 背景: `#ffffff`
- 角丸: 12px
- ボーダー: `1px solid #dadce0`
- シャドウ: なし

### チップ
- 背景: `#ffffff`（デフォルト）/ `#e8f0fe`（選択時）
- テキスト: `#202124` / `#1a73e8`（選択時）
- ボーダー: `1px solid #dadce0`
- 角丸: 8px
- パディング: 6px 16px
- アイコン: 左にMaterial Symbol 18px
- フォント: Roboto 14px / 500

### 入力フォーム
- **Outlined（推奨）**: 白背景、`1px solid #dadce0`ボーダー、4px角丸
- フォーカス: ボーダー`2px solid #1a73e8`、ラベルがブルーに変色して上部に浮上
- エラー: ボーダー`2px solid #d93025`、ヘルパーテキストもレッド
- アイコン付き: 左にMaterial Symbol 24px（`#5f6368`）

### ナビゲーション
- 白背景、下端に`1px solid #dadce0`
- ロゴ: Googleワードマーク左寄せ（4色ロゴ）
- リンク: Roboto 14px / 500、`#5f6368`
- アクティブ: テキスト`#1a73e8`、下線`2px solid #1a73e8`
- CTA: Filledボタン（Google Blue）
- モバイル: ハンバーガー → Material Symbol `menu` アイコン
- ナビアイコン: Material Symbols Outlined 24px

### 特徴的なコンポーネント

**検索バー**
- 白背景、`1px solid #dadce0`ボーダー
- 角丸: 999px（フルピル）——Google検索のシグネチャー
- 左にMaterial Symbol `search` 24px（`#5f6368`）
- フォーカス: シャドウ `0 1px 6px rgba(0,0,0,0.2)` ＋ボーダー除去
- パディング: 12px 16px

**スナックバー/トースト**
- 背景: `#323232`
- テキスト: `#ffffff`、Roboto 14px / 400
- 角丸: 8px
- 下部中央に表示
- アクションリンク: Google Blueのテキストボタン

**タブ**
- テキスト: Roboto 14px / 500
- 非アクティブ: `#5f6368`
- アクティブ: `#1a73e8`＋下部に`2px solid #1a73e8`インジケーター
- アイコン付き: Material Symbol上部＋テキスト下部の縦スタック

## 5. レイアウト原則

### スペーシングシステム
- 基本単位: 8px（4pxの半グリッドも許容）
- スケール: 4px, 8px, 12px, 16px, 24px, 32px, 48px, 64px
- コンポーネント内パディング: 8px, 12px, 16px
- セクション間: 48px, 64px, 80px

### グリッドとコンテナ
- 最大コンテンツ幅: 1200px（マーケティング）/ 840px（記事）
- 12カラムグリッド
- ガター: 24px（デスクトップ）、16px（モバイル）
- アウターマージン: 24px（デスクトップ）、16px（モバイル）
- ヒーロー: 中央1カラム、大きな縦パディング（80–120px）

### 余白の哲学
- **「Googleの白さ」**: 他のテック企業より顕著に広い余白。検索結果ページの広大な白いキャンバスと同じDNA——コンテンツを圧迫せず、目的のアクションへの最短距離を確保
- **コンテンツファーストの密度**: 情報は適切にグルーピングされるが、グループ間は十分な呼吸空間を持つ
- **交互サーフェス**: 白（`#ffffff`）とサーフェスグレー（`#f8f9fa`）の穏やかな交互配色

### 角丸スケール
| レベル | 値 | 用途 |
|--------|-----|------|
| なし | 0px | ディバイダー、フルブリード画像 |
| 極小 | 4px | 入力フィールド、テーブルセル |
| 小 | 8px | チップ、スナックバー、小コンテナ |
| 中 | 12px | カード、ダイアログ |
| 大 | 16px | FAB、シート |
| 特大 | 28px | 大型FAB |
| フル | 999px | ボタン、検索バー、ピル |

## 6. 奥行きと階層

| レベル | 処理 | 用途 |
|--------|------|------|
| L0 | シャドウなし | ベースキャンバス、フラットコンテンツ |
| L1 | `0 1px 2px rgba(0,0,0,0.3), 0 1px 3px 1px rgba(0,0,0,0.15)` | カード、アップバー |
| L2 | `0 1px 2px rgba(0,0,0,0.3), 0 2px 6px 2px rgba(0,0,0,0.15)` | FAB、メニュー |
| L3 | `0 4px 8px 3px rgba(0,0,0,0.15), 0 1px 3px rgba(0,0,0,0.3)` | ダイアログ、モーダル |
| L4 | `0 6px 10px 4px rgba(0,0,0,0.15), 0 2px 3px rgba(0,0,0,0.3)` | ドロワー |
| L5 | `0 8px 12px 6px rgba(0,0,0,0.15), 0 4px 4px rgba(0,0,0,0.3)` | 最大エレベーション |
| フォーカス | `0 0 0 2px #1a73e8`（2pxオフセット） | キーボードフォーカス |
| トーナル | 背景色シフト `#f8f9fa` → `#e8f0fe` | サーフェスエレベーション代替 |

**シャドウの思想**: M3ではシャドウに加えて**トーナルエレベーション**（サーフェス色の明度/彩度シフト）を奥行き表現に使用。ダークテーマではシャドウが見えにくいため、トーナルシフトが主要な奥行きシグナルになる。2層シャドウ（キー+アンビエント）がM3の標準パターン。

## 7. やるべきこと・やってはいけないこと

### やるべきこと
- Google Blue（`#1a73e8`）を唯一のプライマリアクションカラーに
- Material Symbols（Outlined）またはMaterial Design Icons（Outlined）を標準アイコンセットに。選択/アクティブ状態ではFilled（FILL: 1）に切り替え
- アイコンの`opsz`をサイズに合わせて設定（Material Symbols使用時: 20px→opsz 20、24px→opsz 24、48px→opsz 48）
- ボタンはフルピル（999px）——M3 Filledボタンのシグネチャー
- Google Sans（見出し）＋Roboto（本文）の2フォントを厳守
- ステータス色にはソフト背景（`#fce8e6`等）を組み合わせる
- 8pxグリッドに厳格に従う
- 2層シャドウ（キー＋アンビエント）でエレベーション表現

### やってはいけないこと
- ブランド4色（`#4285f4`, `#ea4335`, `#fbbc04`, `#34a853`）をUIアクションカラーに使わない——ロゴ/イラスト/ステータス限定
- Google Sansを本文に使わない——本文は常にRoboto
- ウェイト700をGoogle Sansに使わない——400と500のみ
- Material SymbolsとMaterial Design Icons以外のアイコンセットを混在させない（両者の併用は可）
- 角丸を自由に選ばない——定義済みスケール（0/4/8/12/16/28/999px）から選択
- 単層シャドウを使わない——常に2層（キー＋アンビエント）
- 検索バー以外にフルピル角丸の入力フィールドを作らない——入力は4px角丸
- ブランドカラーのグラデーションを作らない——Googleはソリッドカラーのブランド

## 8. レスポンシブ対応

### ブレークポイント
| 名前 | 幅 | カラム | マージン | 主な変化 |
|------|-----|--------|----------|----------|
| コンパクト | <600px | 4 | 16px | 1カラムスタック、ボトムナビ |
| ミディアム | 600–839px | 8 | 24px | 2カラム開始 |
| エクスパンデッド | 840–1199px | 12 | 24px | 3カラムグリッド |
| ラージ | 1200–1599px | 12 | 24px | フル12カラム |
| エクストララージ | ≥1600px | 12 | 24px | 最大幅、中央配置 |

### 縮退戦略
- ヒーロー: 57px → 45px → 36px → 28px
- ナビ: 水平タブ → ハンバーガー（Material Symbol `menu`）
- カード: 3カラム → 2カラム → 1カラムスタック
- FAB: 大型 → 標準 → ミニ
- タブ: スクロール可能タブに切り替え
- セクション間隔: 80px → 48px → 32px

### ナビゲーションパターン（M3準拠）
| ビューポート | ナビパターン | アイコン使用 |
|--------------|------------|------------|
| コンパクト | ボトムナビゲーションバー | Material Symbols 24px、選択時FILL: 1 |
| ミディアム | ナビゲーションレール（左サイド） | Material Symbols 24px |
| エクスパンデッド+ | ナビゲーションドロワー or トップバー | Material Symbols 24px |

## 9. 実装ガイド

### カラー早見表
- プライマリCTA: `#1a73e8`（Google Blue）
- 背景: `#ffffff`
- セカンダリ背景: `#f8f9fa`
- テキスト: `#202124`（プライマリ）、`#5f6368`（セカンダリ）
- ボーダー: `#dadce0`
- エラー: `#d93025`
- 成功: `#1e8e3e`
- 警告: `#f9ab00`

### Material Icons セットアップ

**A. Material Symbols（推奨）**
```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />

<style>
.material-symbols-outlined {
  font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
}
.material-symbols-outlined.filled {
  font-variation-settings: 'FILL' 1, 'wght' 400, 'GRAD' 0, 'opsz' 24;
}
</style>

<span class="material-symbols-outlined">search</span>
<span class="material-symbols-outlined filled">favorite</span>
```

**B. Material Design Icons（旧版・軽量）**
```html
<!-- CDN -->
<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />
<!-- または npm install material-design-icons -->

<style>
.material-icons { font-size: 24px; color: #5f6368; }
.material-icons.active { color: #1a73e8; }
.material-icons.md-18 { font-size: 18px; }
.material-icons.md-36 { font-size: 36px; }
</style>

<span class="material-icons">search</span>
<span class="material-icons-outlined">favorite</span>
<span class="material-icons active">favorite</span>
```

### プロンプト例
- 「ヒーロー: 白背景。見出し57px Google Sans ウェイト400、行間1.12、字間-0.25px、色#202124。サブ20px Roboto ウェイト400、色#5f6368。Filledボタン（#1a73e8、999px角丸、10px 24px パディング、白テキスト14px Roboto 500）。ボタン左にMaterial Symbol `arrow_forward` 18px。」
- 「カード: 白背景、12px角丸、2層シャドウ（0 1px 2px rgba(0,0,0,0.3), 0 1px 3px 1px rgba(0,0,0,0.15)）。タイトル22px Google Sans 500。本文16px Roboto 400 色#5f6368。下部にOutlinedボタン。」
- 「ナビ: 白背景、下端ボーダー#dadce0。Googleロゴ左寄せ。リンク14px Roboto 500 色#5f6368。アクティブ: #1a73e8＋2px下線。右にFilledボタンCTA。ハンバーガーはMaterial Symbol `menu` 24px。」
- 「検索バー: 白背景、1px solid #dadce0、999px角丸、12px 16px パディング。左にMaterial Symbol `search` 24px 色#5f6368。フォーカスでシャドウ追加＋ボーダー除去。」

### 反復ガイド
1. Google Blue（`#1a73e8`）が唯一のアクションカラー——ブランド4色はUIアクションに使わない
2. Google Sans（見出し）＋ Roboto（本文）の分業を厳守
3. ボタンはフルピル（999px）、カードは12px角丸
4. Material Symbols Outlined（またはMaterial Design Icons Outlined）を標準アイコンに。選択状態でFilled切替
5. Material Symbols使用時はopsz軸をサイズに合わせる（20/24/36/48）。Material Design Icons使用時はfont-sizeで制御
6. 2層シャドウ（キー＋アンビエント）でエレベーション
7. 8pxグリッドを厳守
8. ステータス色はソフト背景とペアで使用
