# 作業ルール

## 編集対象

- 特別な指定がない限り、編集対象は **low profile 版**（`config/meteorite40_low.keymap` / `config/meteorite40_low.conf` / `boards/shields/meteorite40_low/`）。
- 通常版 (`meteorite40`) を変更する場合はユーザーが明示的に指示する。

## コミットとプッシュ

- ビルドは GitHub Actions (`.github/workflows/build.yml`) で行うため、ローカルビルドはしない。
- ブランチは切らず **main に直接コミットして良い**。実装が終わったら即 `git push` する。
- push 後は **直近の GitHub Actions の実行が終わるまで待つ**。`gh run watch` などで完了を確認してから次の作業に進む / 結果をユーザーに報告する。
- 失敗していたら原因を確認して修正コミット → 再 push → また待つ。
