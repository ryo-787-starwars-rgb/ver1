# MISSION REACHER v2.2 — BODY SIMULATOR

GitHub Pages対応の静的PWA。既存の `mission-reacher-v2` localStorage キーを維持します。

## 更新
1. 旧アプリ DATA からJSONバックアップを書き出す。
2. このフォルダの6ファイルをGitHubリポジトリのルートにアップロードし、同名ファイルを上書きする。
3. GitHub Pagesのデプロイ完了後、iPhoneでページを再読み込み。古い表示の場合はSafariの再読み込み・ホーム画面アプリの再起動を試す。

## 追加内容
- BODYタブ：イラスト調人体シミュレーター（正面・側面・背面）
- CURRENT / TARGET / FUTURE、現在と目標の並列比較
- 胸・肩・背中・腕・脚・体脂肪率の調整、STATS測定値との連動
- SIGNATURE PROGRAMS：曜日と「軍人仕様」の表示を削除。4プログラムの内容は維持。
- BODY PART、COMBINATION、CUSTOM、食事・PFC、成長グラフ、目標、JSONバックアップは維持。

**注意**：モデルは模式図であり、実測の体型や将来の姿を精密に推定するものではありません。FUTUREは十分な体脂肪率記録がある場合のみ単純傾向を反映します。
