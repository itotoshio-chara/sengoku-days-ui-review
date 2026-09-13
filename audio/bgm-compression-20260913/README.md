# BGM圧縮の聞き比べ

各曲の8〜16秒を、同じ音量・同じ24bit PCM WAV形式で比較します。圧縮後はゲーム用MP3全曲をデコードしてから同じ区間を切り出しています。再エンコードの重なりや音量補正はありません。比較用WAVの容量が同じなのは意図的で、ゲーム配信には小さいMP3のみを使います。

|曲|原音|圧縮後|
|---|---|---|
|春夏|[原音8秒](https://raw.githubusercontent.com/itotoshio-chara/sengoku-days-ui-review/refs/heads/codex/review-bgm-compression-20260913/audio/bgm-compression-20260913/spring-original.wav)|[MP3圧縮後8秒](https://raw.githubusercontent.com/itotoshio-chara/sengoku-days-ui-review/refs/heads/codex/review-bgm-compression-20260913/audio/bgm-compression-20260913/spring-compressed.wav)|
|最終決戦|[原音8秒](https://raw.githubusercontent.com/itotoshio-chara/sengoku-days-ui-review/refs/heads/codex/review-bgm-compression-20260913/audio/bgm-compression-20260913/final-battle-original.wav)|[MP3圧縮後8秒](https://raw.githubusercontent.com/itotoshio-chara/sengoku-days-ui-review/refs/heads/codex/review-bgm-compression-20260913/audio/bgm-compression-20260913/final-battle-compressed.wav)|

一度に1つだけ再生し、同じ端末・音量で交互に聴いてください。笛や高音の響き、打楽器、残響を確認してください。MP3は非可逆圧縮のため同一音ではありません。サンプル長とループ境界は機械的に検証済みですが、実聴による音質判定・iPhone実機の音声出力は未確認です。

全曲容量：春夏6,513,276→930,501 bytes、最終決戦ループ7,938,044→1,757,104 bytes。設定はFFmpeg7.1 libmp3lame VBR q0、Xing/LAME gaplessタグ、原音のsample rate/channels維持。音楽全7本は48,291,512→6,489,639 bytes。レビュー資産のみで本番への混入はありません。
