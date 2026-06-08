# fizz-stream-sentence-parser

**Fizz** (AITuber system in [Almide](https://github.com/almide/almide)) — §3 brain 部品。

LLM 出力 → 文 + `[emotion]/[fx]/[hair]` タグ切り出し。`parse_all` / `feed` (ストリーミング用 remainder 返し)。文字リストで処理しマルチバイト安全。

責務は一行で、入力 → 出力が型で言い切れる単位 (openaituber `docs/almide-component-breakdown.md` §3)。

## Install

```toml
[dependencies]
fizz_stream_sentence_parser = { git = "https://github.com/Aid-On/fizz-stream-sentence-parser", tag = "v0.1.0" }
```

## Tests

```bash
almide test
```

純ロジックなのでネットワーク・API キー不要でテストできる。
