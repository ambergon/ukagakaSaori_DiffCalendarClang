# ukagakaSaori_DiffCalendarClang
伺か/SSPで使用できるSAORIです。
差の日数を取得することができます。
```
＃ A - B = 差
差の日数 = （DiffCalendar,A年,A月,A日,B年,B月,B日）
```

以前C#で書いたものには、ゴーストのアンインストール等でSAORIが残ってしまう問題があったのでCで書き直しました。
前回 : [GitHub - ambergon/ukagakaSaori_DiffCalendar](https://github.com/ambergon/ukagakaSaori_DiffCalendar)


## 導入
satori.dllのあるディレクトリにSaoriフォルダを追加。
Saoriディレクトリの中にukagakaSaori_DiffCalendar.dllを保存。
saori_conf.txtの@SAORI以降に下記を追記
```
＠SAORI
＃呼び出し名,ディレクトリ/名前.dll
DiffCalendar,Saori/ukagakaSaori_DiffCalendar.dll
```


## 使い方
前回のものと一部変更されました。
全角数字を半角数字に変換するため、事前にZen2Hanを撃つ必要がなくなりました。
これはShift-JIS環境のみ変換されます。(SATORIユーザは気にしないでよいということ。)
```
＊0headつつかれ
：計算
＃（DiffCalendar,A年,A月,A日,B年,B月,B日）
差の日数 = （DiffCalendar,2023,5,1,2021,1,1）
＃-＞ 850
```


## License
このプログラムを使ったいかなる問題や損害に対して、私は責任を負いません。
また、ゴーストなどに同梱して配布していただいて構いません。

## Author
ambergon

