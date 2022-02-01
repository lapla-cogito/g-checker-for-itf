# g-checker-for-itf
ITF の卒業要件を確認したい。(今はcoins20 だけ)

提供されているプログラム、またそのプログラムによる実行結果に関する保証はできかねます。


# usage

```
python3 main.py -i target_csv_file
```

で実行できます。
複数ファイルを引数に与えることができ、その場合は連続して判定が行なわれます。
`target csv file` は twins の成績ページからダウンロードしたファイル (UTF, CSV) を想定しています。

```
options:
  -h, --help            show this help message and exit
  -i INPUT, --input INPUT
                        target file from twins (UTF-8, CSV)
  -r REQUIREMENTS, --requirements REQUIREMENTS
                        requirements file
  -g, --gpa             print GPA Flag
  -d, --drop            print drop credit unable Flag
  -n, --name            print name and id, able Flag
```

# test 

```
python3 main.py -i sample.csv -r coins20.json
```


で予め用意されたサンプルで動作を確認することが出来ます。

# viewer

```
python3 -s -i target_csv_file
cd tani
npm install
npm start
```

[http://localhost:3001/](http://localhost:3001/) にアクセスすると確認できます。

# image

<img width="1358" alt="イメージ画像(CUI)" src="https://user-images.githubusercontent.com/65126083/151887795-b8b7bca4-b8bc-4822-ad60-e7e721b23805.png">
<img width="1358" alt="イメージ画像(GUI)" src="https://user-images.githubusercontent.com/65126083/151980981-3f7aa1e0-2a16-40d8-a243-615a3f736f9a.png">
