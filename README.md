# taiyo8911.github.io

SolSEのサイト（ハブ）と、アプリの公式ページです。

- 公開URL：https://taiyo8911.github.io

## 構成

| パス | 内容 |
|---|---|
| `index.html` | ハブ（自己紹介・各種リンク） |
| `style.css` | サイト全体の共通デザイン |
| `404.html` | 存在しないURLを開いたときのページ |
| `favicon.svg` / `apple-touch-icon.png` | ブラウザのタブ・ホーム画面のアイコン |
| `ogp.png` | SNSで共有したときのカード画像（1200×630） |
| `apps/アプリ名/` | アプリの公式ページ（紹介・FAQ・問い合わせ・プライバシーポリシー） |
| `apps/_template/` | 新しいアプリ用のひな形（`_` で始まるため公開されない） |

Webアプリ本体は、それぞれのリポジトリのGitHub Pagesで公開しています（`taiyo8911.github.io/リポジトリ名/`）。

## アプリを追加するとき

1. `apps/_template/` をコピーして `apps/アプリ名/` にする
2. `index.html` のアプリ名・説明・リンクなどを書き換え、`icon.png` を置く
3. `SUPPORT_EMAIL` をサポート用のメールアドレスに置き換える
4. 必要ならハブ（`index.html`）にリンクを追加する
5. push する（1〜2分で反映）

## App Store Connect に登録するURL

| 項目 | URL |
|---|---|
| サポートURL | `https://taiyo8911.github.io/apps/アプリ名/` |
| プライバシーポリシーURL | `https://taiyo8911.github.io/apps/アプリ名/#privacy` |
| マーケティングURL | 空欄 |
| 利用規約 | Apple標準EULAを使用 |

※ プライバシーポリシーURL・サポートURLは、新しいバージョンを申請するときにしか変更できない。

## 旧URLからの転送

以前のサポートページは、各アプリのリポジトリの `docs/index.html` で新しいページへ転送している。

| 旧URL | 転送先 |
|---|---|
| `/KraepelinApp/` | `/apps/kraepelin/` |
| `/touchNumbers/` | `/apps/tappun/` |
| `/Quick-Reversi/` | `/apps/quick-reversi/` |
| `/Schedule_Clock/` | `/apps/schedule-clock/` |
| `/SecretNumbers/` | `/apps/number-hunt/` |

転送用の `docs/index.html` は消さない（App Storeに旧URLが残っているアプリがあるため）。

## 問い合わせ

各アプリページのボタンから、件名にアプリ名が入ったメールで受け付ける。

## ルール

- アプリのフォルダ名は英小文字とハイフンのみ。一度決めたら変えない
- Webアプリのフォルダ名は、本体のリポジトリ名とそろえる
- `apps` という名前のリポジトリを作らない（URLが衝突するため）
- このリポジトリの直下に、ほかのリポジトリと同じ名前のフォルダを作らない
- GitHubのユーザー名は変えない（すべてのURLが変わるため）
- このリポジトリはPublic。サイトのファイル以外（メモ・パスワード等）は置かない
