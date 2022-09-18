# SNS分析によるイベントレコメンド
 
# Requirements
 
```bash
pip install requirements.txt
```

単語の類似度計算に用いる日本語 Wikipedia エンティティベクトルのダウンロード

解凍したファイル（entity_vector）をプロジェクトディレクトリ直下に置く
```bash
wget http://www.cl.ecei.tohoku.ac.jp/~m-suzuki/jawiki_vector/data/20170201.tar.bz2
tar -jxvf 20170201.tar.bz2
```

# Methods


イベントモデルの作成
```bash
attendeeCharacter(event_name)　#event_name：イベントの名前（文字列）
```

ユーザの興味とイベント特性の類似度の算出方法
```bash
eventRecommendation(user_name, attendee)　#user_id：利用者を示すアカウントid、attendee：イベントモデル
```
