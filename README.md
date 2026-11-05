# MISSION REACHER — COMPLETE (2026-11)

GitHub Pages (`ver1`) 用PWA。ZIP内のファイルをリポジトリのルートへ上書きしてください。

## 更新前に必ずバックアップ
旧アプリ → DATA → JSON書き出し → `.json` を保存。ZIP解凍後のファイルをGitHubへアップロードしてコミット。新アプリで記録が見えない場合は DATA → JSON復元。復元は現在のデータを置き換えるので、先に現在のデータも書き出してください。

## 主な機能
- TRAIN: 7部位×8プラン、組み合わせ、4種のSIGNATURE、自由入力・代替種目、セットログ
- FOOD: 100種類以上の食材検索、卵は個、納豆はパック、食パンは枚、牛乳はmL、その他はg。プロテイン粉末は1杯のPFC/kcalと杯数
- STATS: 朝体重（推奨）・夜体重（任意）・朝7日移動平均・その他身体測定、種目別推移
- GOALS: 体重の予測は朝7日移動平均を使用。データ不足時は予測準備中
- DATA: JSONエクスポート・インポート
- BODY SIMULATOR・食費管理UIなし。記録はブラウザのlocalStorageに保存

### 注意
食材の栄養値や個数換算は概算。卵は可食部50g/個、納豆45g/パック、食パン60g/枚、牛乳は1mL≈1g。商品ラベルを優先してください。iPhone実機検証は未実施です。


## PFC dashboard update
FOOD画面に日別の目標との差・不足・超過・達成表示を追加。目標は既存の体重・活動量・減量/維持/増量設定から計算。既存のlocalStorageキーとJSONバックアップ形式を維持。


### 2026-11-05 workout update
- Add/remove exercises individually, reorder with up/down arrows.
- Add/remove individual sets, edit each set independently.
- Recommendations from last 8 sessions with completed sets for the exact exercise name, including uncertainty and optional apply.
- Recommendations exclude the current session, keep completed sets unchanged, and preserve previous sessions.


## トレーニング時刻・カロリー・カレンダー
- プラン開始時に開始時刻を保存。終了ボタンで終了時刻を保存し、経過分数を計算。編集を閉じるボタンは記録を削除しません。
- 完了したセット数から運動強度（3.5/4.5/5 MET）を概算し、MET×3.5×体重kg÷200×分数で消費kcalを推定します。運動消費の計算はセッション終了後のみ。測定値ではありません。
- FOODでは推定運動消費を別表示。チェックを入れた場合のみ、摂取カロリー目標と炭水化物目標に加算します。日常活動込みの目標と二重計上しないよう注意。
- CALタブで月別の日付を選び、当日の食事・PFC・トレーニング・時刻・セットを確認できます。
- 旧版データはそのまま読み込みますが、旧記録には開始・終了時刻がないため消費kcalを遡及推定しません。
- 更新前にDATAからJSONをエクスポートしてください。


### CAL身体情報統合
日付選択で食事・PFC・筋トレ・身体測定を確認。朝晩体重、体脂肪率、筋肉量、胸囲、腹囲、腕周りをその日付で追加・編集できます。過去の食事は日付を保持してFOOD画面に移動。筋肉量はSTATSにも追加。既存の保存キーを維持しています。
