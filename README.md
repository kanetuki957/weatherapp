# weatherapp
日本国内の都市を入力すると、現在の天気と週間予報を取得して表示する React 製アプリです。   背景色が天気に応じて変化する、シンプルで見やすい天気アプリになっています。

#主な機能：
<br>
・都市名で現在の天気を検索  
・5日間の週間予報を表示  
・天気に応じて背景カラーが自動で変化  
・都市名の入力ミス時にはエラーメッセージを表示  
・日本語で天気情報を取得（OpenWeatherMap API 利用）

#使用技術：バージョン
<br>
Node.js   20.x<br>
フロントエンド:React(Vite) 18.x<br>
言語:JavaScript/JSX 5.x<br>
API:[OpenWeatherMap API](https://openweathermap.org/api)<br>
スタイル:CSS(カスタムクラスで背景変化)
<br>
#セットアップ方法
<br>
①リポジトリをクローン
git clone https://github.com/ユーザー名/react-weather-app.git
cd react-weather-app
<br>
②依存関係のインストール
<br>
npm install

③.env ファイルを作成
<br>
プロジェクト直下に .env を作り、以下を記述します：<br>
VITE_API_KEY=あなたのOpenWeatherMapのAPIキー
・APIキーは OpenWeatherMap公式サイトで無料登録すると取得できます。

<br>
④開発サーバーの起動
<br>
npm run dev

#背景カラーの変化
<br>
天気	｜カラーイメージ<br>
晴れ	｜明るい黄色〜オレンジ<br>
曇り	｜グレー系<br>
雨	　｜青系<br>
雪	　｜白〜水色系<br>
その他	｜淡いグレー<br>

#ディレクトリ構成
<br>
src/
├── App.jsx               メインコンポーネント
├── WeatherCard.jsx       現在の天気カード
├── ForecastCard.jsx      週間予報カード
├── cityMap.json          日本語 → 英語変換用データ
├── App.css               デザイン全般
└── assets/               画像・アイコン類

#今後の拡張予定
<br>
・現在地から自動で天気を取得
・天気に合わせたコメント表示
・世界の都市への対応
・夜間テーマ対応




