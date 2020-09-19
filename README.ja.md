[en](./README.md)

# Shell.JapaneseFirstNameGenerator.20200919111358

　日本人の名字を除く名前を重複せずランダムに生成する。性別も出力する。

# デモ

```sh
$ jfn.sh
しげまさ	重誠	M
あさはる	朝晴	M
れんいちろう	錬一郎	M
しょうぞう	章三	M
かいま	貝真	M
あきたか	明謙	M
とうし	桃志	M
のりと	慰翔	M
あおや	青矢	M
てんが	天雅	M
せいたろう	誠多郎	M
ゆきよ	幸代	M
かいき	加衣貴	M
しんり	心琉	M
のりお	法男	M
うみの	うみの	F
てるこ	耀子	F
かなみ	佳並	F
あきね	諒寧	F
ゆあら	由明羅	F
ほづき	步月	F
すずほ	珠々帆	F
みきほ	美祈歩	F
りさ	鈴桜	F
ゆうあ	宥亜	F
ふきえ	富貴惠	F
きょうな	杏那	F
りい	莉惟	F
のこ	乃瑚	F
おとえ	音絵	F
```
```sh
$ time jfn.sh
...
real	0m1.421s
user	0m1.389s
sys	0m0.585s
```

# 特徴

* `読み\n表記\n性別`の書式で出力する
* 出力件数を指定できる
* 条件指定して抽出するサブコマンドがある

# 開発環境

* <time datetime="2020-09-19T11:13:55+0900">2020-09-19</time>
* [Raspbierry Pi](https://ja.wikipedia.org/wiki/Raspberry_Pi) 4 Model B Rev 1.2
* [Raspbian](https://ja.wikipedia.org/wiki/Raspbian) buster 10.0 2019-09-26 <small>[setup](http://ytyaru.hatenablog.com/entry/2019/12/25/222222)</small>
* bash 5.0.3(1)-release

```sh
$ uname -a
Linux raspberrypi 4.19.97-v7l+ #1294 SMP Thu Jan 30 13:21:14 GMT 2020 armv7l GNU/Linux
```

# インストール

```sh
git clone https://github.com/ytyaru/Shell.JapaneseFirstNameGenerator.20200919111358
```

# 使い方

```sh
cd Shell.JapaneseFirstNameGenerator.20200919111358/src
./jfn.sh
```

# 注意

## 既知のバグ

* `-n`の値を`2938`以上にすると`	-e F	`など不正な行が出力される: [note](https://github.com/ytyaru/Shell.JapaneseFirstNameGenerator.20200919111358/blob/master/note/bug/1.md)

## 仕様変更

* 男女比ランダムを削除した
    * [前の版](https://github.com/ytyaru/Shell.JapaneseFirstNameGenerator.20200918080000)からサブコマンド`g`の引数`-r`の値`r`を削除した: [note](https://github.com/ytyaru/Shell.JapaneseFirstNameGenerator.20200919111358/blob/master/note/change_spec/1.md)

# 著者

　ytyaru

* [![github](http://www.google.com/s2/favicons?domain=github.com)](https://github.com/ytyaru "github")
* [![hatena](http://www.google.com/s2/favicons?domain=www.hatena.ne.jp)](http://ytyaru.hatenablog.com/ytyaru "hatena")
* [![mastodon](http://www.google.com/s2/favicons?domain=mstdn.jp)](https://mstdn.jp/web/accounts/233143 "mastdon")

# ライセンス

　このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)

