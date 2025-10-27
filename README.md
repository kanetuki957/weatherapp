# weatherapp
日本国内の都市を入力すると、現在の天気と週間予報を取得して表示する React 製アプリです。   背景色が天気に応じて変化する、シンプルで見やすい天気アプリになっています。

#主な機能：
・都市名で現在の天気を検索  
・5日間の週間予報を表示  
・天気に応じて背景カラーが自動で変化  
・都市名の入力ミス時にはエラーメッセージを表示  
・日本語で天気情報を取得（OpenWeatherMap API 利用）

#使用技術：バージョン
Node.js   20.x
フロントエンド:React(Vite) 18.x
言語:JavaScript/JSX 5.x
API:[OpenWeatherMap API](https://openweathermap.org/api)
スタイル:CSS(カスタムクラスで背景変化)

#セットアップ方法
①リポジトリをクローン
git clone https://github.com/ユーザー名/react-weather-app.git
cd react-weather-app

②依存関係のインストール
npm install

③.env ファイルを作成
プロジェクト直下に .env を作り、以下を記述します：
VITE_API_KEY=あなたのOpenWeatherMapのAPIキー
・APIキーは OpenWeatherMap公式サイトで無料登録すると取得できます。

④開発サーバーの起動
npm run dev

#背景カラーの変化
天気	｜カラーイメージ
晴れ	｜明るい黄色〜オレンジ
曇り	｜グレー系
雨	　｜青系
雪	　｜白〜水色系
その他	｜淡いグレー

#ディレクトリ構成
src/
├── App.jsx               メインコンポーネント
├── WeatherCard.jsx       現在の天気カード
├── ForecastCard.jsx      週間予報カード
├── cityMap.json          日本語 → 英語変換用データ
├── App.css               デザイン全般
└── assets/               画像・アイコン類

#今後の拡張予定
・現在地から自動で天気を取得
・天気に合わせたコメント表示
・世界の都市への対応
・夜間テーマ対応




