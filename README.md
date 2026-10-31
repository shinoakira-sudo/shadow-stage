# Shadow Stage

TEDトーク（YouTube）でシャドーイングを練習する、1ファイルのWebアプリです。

- 公開ページ: GitHub Pages（このリポジトリの `index.html`）
- 機能: YouTube再生 / スクリプトの表示・ぼかし・非表示 / 行タップで該当場面へ / ループ / 速度0.5〜1.5x / 録音と音声認識による単語一致の分析 / 学習記録（ブラウザ内のみ）
- スクリプト（文字起こし）は各自が YouTube の「文字起こしを表示」からコピーして貼り付けます。リポジトリには含みません。

更新は `index.html` を差し替えて push するだけです。

## よみスタ（`yomista/`）

小学生の音読アプリ「よみスタ」のウェブ版です（Claude の画面ではマイクが使えないため、録音して評価する「音読チェック」はこちらで使います）。

- 公開ページ: GitHub Pages の `yomista/`（`https://shinoakira-sudo.github.io/shadow-stage/yomista/`）
- 中身: `yomista/index.html`（1ファイルのアプリ）と、付属のおはなし40パートの読み上げ音声 `yomista/audio/*.mp3`（VOICEVOX:No.7）
- おはなしの本文は青空文庫（著作権の切れた作品）から。記録はブラウザ内のみ。音読チェックの評価は Supabase の Edge Function（合言葉つき）経由で Gemini に送ります。
- 検索エンジンには載せない設定（`noindex`）です。

更新は `yomista/index.html` を差し替えて push するだけです。
