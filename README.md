# ASCIItoHiragana

1バイトフォント (キーボードに印字されたひらがなが入力されるタイプのフォント) を，ローマ字入力できるように変換する FontForge スクリプト `1to2-h.pe`．
これ単体では動作せず，[FontFotge](https://fontforge.org/en-US/) が必要です．

これを作ったのは2016年なんですが，FontForge の [Scripting ドキュメント](https://fontforge.org/docs/scripting/scripting.html) に「`.pe` はレガシーです」って書かれてますね...
> FontForge includes two interpreters so you can write scripts to modify fonts. One of these interpreters is python, one is a legacy language I came up with. 
>
>  “py” means use the python interpreter, “ff” or “pe” means use the old interpreter

# 使い方
```
$ fontforge -script 1to2-h.pe [SOURCE-FONT]
```

出力されるフォントのファイル名は `[SOURCE-FONT]_ed.ttf` となります．

詳しい情報は[僕のブログ](https://lookbackmargin.blog/2016/02/21/52157254/)に (そんなに詳しくないかもしれないけど)
