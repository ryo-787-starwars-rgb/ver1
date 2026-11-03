# MISSION REACHER v2.1

## 変更点
- FOOD: 食費入力と食費集計を撤去。目標体型に応じてPFCと摂取カロリーを自動提案
- 体重・目標体重・活動量・減量/維持/増量を選択
- iPhone向け入力欄・文字・余白・ナビゲーションを調整
- 既存のMILITARY/BODY PART/COMBINATION/CUSTOM、筋力記録、グラフ、GOALSを維持
- DATAタブにJSONバックアップ/復元を維持

## 注意
- 予測PFCは体重×活動係数に基づく初期推定であり、医学的な個別処方ではありません。
- 最新の身体記録がある場合、そちらの体重を使います。
- データは既存の localStorage キー mission-reacher-v2 に保存され、以前の記録を引き継ぎます。
- 更新前に DATA タブからJSONをバックアップしてください。
- GitHub PagesではZIPを解凍し、6ファイルをリポジトリ直下にアップロードしてください。
