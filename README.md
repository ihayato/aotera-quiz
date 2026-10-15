# あおてら！ クイズ問題集

日本語のクイズ問題、**9,965問**。
無料で、商用でも使えます（CC BY-SA 4.0）。

クイズゲーム「[あおてら！](https://vibe.co.jp/izayoi/)」で、実際に出している問題です。

**ブラウザで見る → [あおてら！問題集](https://vibe.co.jp/aotera/mondai/)**
ジャンル・形式・難しさで絞り込んだり、言葉で探したりして読めます。

## 中身

| ジャンル | 問題数 |
|---|---:|
| 文系の学問 | 1,819 |
| ライフスタイル | 1,745 |
| スポーツ | 1,654 |
| アニメ・ゲーム | 1,620 |
| 理系の学問 | 1,583 |
| 社会 | 1,544 |

| 形式 | 問題数 | どんな問題か |
|---|---:|---|
| ○× | 2,446 | 文が正しいか答える。×の問題には「正しくは」が付いています |
| 順番当て | 1,808 | 4つを、年代や大きさの順に並べる |
| 四択 | 1,708 | 4つの中から1つ選ぶ |
| 文字パネル | 1,525 | 12枚の文字から選んで答えを作る |
| 並べ替え | 1,440 | バラバラの文字を並べて答えを作る |
| 連想 | 1,038 | 5つのヒントから、4つの中の1つを当てる |

難しさは1〜5の5段階です。

## ファイル

| ファイル | 中身 |
|---|---|
| `data/all.csv` | 全問。Excel などの表計算で開けます |
| `data/all.jsonl` | 全問。1行に1問 |
| `data/genre/*.jsonl` | ジャンルごと |
| `data/flat.jsonl` | 全問。どの形式も同じ項目にそろえた版 |
| `docs/FORMAT.md` | 項目と形式の説明 |

## 1問の例

```json
{
  "id": "551b5ce7d1e59893",
  "genre": "life",
  "format": "maru",
  "difficulty": 1,
  "body": { "text": "ジーンズに使われるデニム生地は、主に絹を原料として作られる。" },
  "answer": false,
  "note": "ジーンズのデニム生地は、主に綿（コットン）を原料に作られる。",
  "source_url": "https://ja.wikipedia.org/wiki/デニム",
  "as_of": "2026-10-07",
  "expires": null,
  "version": 1
}
```

```json
{
  "id": "1f53b71f47c286bb",
  "genre": "rikei",
  "format": "rensou",
  "difficulty": 2,
  "body": {
    "hints": ["1921年ノーベル物理学賞", "受賞理由は光電効果の説明", "1905年に論文を連発", "E=mc²を導いた", "相対性理論の提唱者"],
    "choices": ["ハイゼンベルク", "プランク", "ボーア", "アインシュタイン"]
  },
  "answer": "アインシュタイン"
}
```

（2問目は `note` から下を省いています）

ほかの形式は [docs/FORMAT.md](docs/FORMAT.md) にあります。

## 作り方

- 生成AIで問題を作り、別の生成AIがウェブの資料と照らして事実を確かめました。
- そのあと、さらに2回点検しています。答えが1つに決まるか、問題文に答えが見えていないか、時間がたつと答えが変わらないか。
- 点検で引っかかった問題は入れていません。公開の前にも、引用や答えの手がかりが気になる問題を外しました。
- どの問題にも、確かめた資料（`source_url`）と確かめた日（`as_of`）が付いています。資料そのものの文章のライセンスは、それぞれの資料に従います。

## 使うときの決まり

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.ja) です。

- 自由に使えます。アプリやゲーム、授業、AIの評価や学習にも。売り物に入れても大丈夫です。
- 使ったところに、この問題集の名前・リンク・ライセンスを書いてください。
- 問題を直したり作り変えたりしたときは、そう書いてください。ほかの人が直した版を使うときは、その人の表示も残してください。
- 直したり作り変えたりした問題を配るときは、同じ CC BY-SA 4.0（または CC が認めた互換ライセンス）で配ってください。問題を使うアプリやゲームそのものまで同じライセンスにする必要はありません。

書き方の例:

```
問題: あおてら！ クイズ問題集 https://github.com/ihayato/aotera-quiz
ライセンス: CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/deed.ja

問題: あおてら！ クイズ問題集 https://github.com/ihayato/aotera-quiz を一部改変
ライセンス: CC BY-SA 4.0 https://creativecommons.org/licenses/by-sa/4.0/deed.ja
```

問題の中にある作品のせりふや書き出しなどの短い引用は、元の作品のものです。このライセンスで許すものではありません。

## 間違いを見つけたら

[Issue](https://github.com/ihayato/aotera-quiz/issues/new/choose) で教えてください。問題の `id` があると助かります。
直した問題は、次の版に入ります。

## 版

| 版 | 問題数 |
|---|---:|
| 2026.10 | 9,965 |

問題は順に増やしていきます。

© 2026 合同会社日本の田舎は資本主義のフロンティアだ

---

## English

**Aotera Quiz Dataset** — 9,965 Japanese trivia questions, free for any use including commercial (CC BY-SA 4.0).

- Drawn from the live questions of the quiz game [Aotera!](https://vibe.co.jp/izayoi/).
- Browse and search all questions in your browser: [vibe.co.jp/aotera/mondai](https://vibe.co.jp/aotera/mondai/) (Japanese).
- 6 genres (humanities, lifestyle, sports, anime & games, science, society) × 6 formats (true/false, ordering, 4-choice, letter panel, letter scramble, 5-hint association). Difficulty 1–5.
- Written by generative AI, fact-checked by a different AI against web sources, then reviewed twice more (single correct answer, no answer leaks in the question, no time-sensitive drift). Every question links its source (`source_url`) and the check date (`as_of`).
- Use `data/all.jsonl` (original structure), `data/flat.jsonl` (same fields for every format) or `data/all.csv`. Field details: [docs/FORMAT.md](docs/FORMAT.md).
- Please credit: `Aotera Quiz Dataset https://github.com/ihayato/aotera-quiz (CC BY-SA 4.0)`, and say so if you changed the questions. Share modified questions under CC BY-SA 4.0; the app or game that uses them does not need to.
- Short quotations from works (lines, opening sentences) inside some questions belong to their original works and are not licensed here.
- Found a mistake? Open an [issue](https://github.com/ihayato/aotera-quiz/issues/new/choose) with the question `id`.
