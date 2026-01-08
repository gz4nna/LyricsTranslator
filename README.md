由于有批量翻译歌词文件的需求，为了自动化处理，于是考虑到通过这个脚本去调用模型翻译。

## 运行依赖

1. 环境和库：`python`，`openai`，`tqdm`
2. 需要将 `client` 替换为您自己的 LLM 服务地址和 api key

## 使用方法

将待翻译的 `.lrc` 文件放在 `./lists` 文件夹下面，运行 `LyricsTranslator.ipynb`，输出内容放置在 `./output` 文件夹下

## 其他说明

1. 目前提示词设定为英译中
2. 歌词中的歌曲元信息设定在 `meta_keywords` 中过滤
3. AI 可能会出错，可以通过调整 model，prompt 和 temperature 等提高翻译质量，但是最终成果务必由人类检查
