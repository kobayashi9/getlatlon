# 概要
Google Mapsの過去のタイムライン情報から以下のデータのみを取得する。
- 自分が訪れた位置データ
- 訪れたランドマークの位置データ

# 使い方
1. Google Mapsの過去のタイムライン情報(zipファイル)を取得する。
1. 「1.」で取得したファイルのパスをコマンドライン引数に指定して実行する。（以下）
    ```bash
    $ python3 getlatlon.py xxxxxx.zip
    ```
1. 以下フォーマットのjsonファイルが出力される。
```json
[
    {
        "datetime": "xxxxx",
        "latitude": "yyyyy",
        "longitude": "zzzzzz",
    },
    {
        "datetime": "xxxxx",
        "latitude": "yyyyy",
        "longitude": "zzzzzz",
    },
    {
        "datetime": "xxxxx",
        "latitude": "yyyyy",
        "longitude": "zzzzzz",
    },
    {
        "datetime": "xxxxx",
        "latitude": "yyyyy",
        "longitude": "zzzzzz",
    }
]
```
