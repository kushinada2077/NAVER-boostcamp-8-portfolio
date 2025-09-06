# 🔎 Code Clashのご紹介

![Code Clash](https://user-images.githubusercontent.com/43944581/281335955-aa2882f9-c134-40a3-b506-b7ab42815543.png)

Code Clashは、ありきたりなアルゴリズム対戦プラットフォームではありません。アイテムを使用して相手を妨害するアーケードゲームの要素と、アルゴリズム対戦を融合させた新しい形のリアルタイム対戦ゲームです。
ユーザーはルームを作成して他のプレイヤーと参加し、リアルタイムでアーケードスタイルのプログラミング対戦（PS）を楽しむことができます。

勝率や正答率といった指標を通じて健全な競争を促しつつ、少し堅苦しくなりがちなプログラミング対戦に「アイテム」という遊び心を加えることで、より親しみやすく、誰もが楽しめるサービスを目指しました。

▼ Code Clashを体験する <br>
https://codeclash.duckdns.org

# 👨‍👩‍👧‍👦 チームメンバー

| J091\_イグンソン                                                    | J096\_イドンハ                                                  | J152\_ジヒョンベ                                             | J167\_ヒョンチャヌ                                           |
| ------------------------------------------------------------------- | --------------------------------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------ |
| ![img](https://avatars.githubusercontent.com/u/79559361?v=4)         | ![img](https://avatars.githubusercontent.com/u/111179843?v=4)   | ![img](https://avatars.githubusercontent.com/u/43944581?v=4)    | ![img](https://avatars.githubusercontent.com/u/77053595?v=4)  |
| [@Geun Seong Lee](https://github.com/LEEGURTS)                      | [@kushinada](https://github.com/kushinada2077)                  | [@ruok](https://github.com/ruokic)                             | [@ChanWoo Hyun](https://github.com/h9661)                    |

# 🚀 担当した役割と貢献

1.  **サーバーアーキテクチャの設計とリアルタイム通信環境の構築**
    > Nginxをリバースプロキシとして導入し、静的・動的リクエストを分離することでAPIサーバーの負荷分散を行いました。また、Polling方式に比べてサーバーリソースとパフォーマンスに利点があるWebSocket技術を採用し、遅延のないリアルタイムなチャット及びゲーム環境の構築に成功しました。
    > * **(詳細な技術解説: [NginxでのHTTPS設定](https://github.com/kushinada2077/NAVER-boostcamp-8-portfolio/wiki/Nginx%E3%81%A7%E3%81%AEHTTPS%E8%A8%AD%E5%AE%9A) / [WebSocketの選定理由](https://github.com/kushinada2077/NAVER-boostcamp-8-portfolio/wiki/%E3%83%AA%E3%82%A2%E3%83%AB%E3%82%BF%E3%82%A4%E3%83%A0%E9%80%9A%E4%BF%A1%E6%8A%80%E8%A1%93%E3%81%AE%E6%AF%94%E8%BC%83%E3%81%A8WebSocket%E3%81%AE%E9%81%B8%E5%AE%9A%E7%90%86%E7%94%B1))**

2.  **主体的な役割再分配によるチーム開発の生産性向上**
    > ペアプログラミングの過程で生じた開発スタイルの違いやコミュニケーションの非効率を解決するため、私がWebSocket機能実装のオーナーシップを持つことを提案し、役割を再分配しました。これにより、チームメンバーの業務集中度を高め、コードの一貫性を確保することで、チーム全体の開発生産性を大きく向上させた経験があります。
    > * **(課題解決のプロセス: [チーム開発プロセスの改善](https://github.com/kushinada2077/NAVER-boostcamp-8-portfolio/wiki/%E3%83%81%E3%83%BC%E3%83%A0%E9%96%8B%E7%99%BA%E3%83%97%E3%83%AD%E3%82%BB%E3%82%B9%E3%81%AE%E6%94%B9%E5%96%84%E3%81%A8WebSocket%E5%AE%9F%E8%A3%85%E3%81%AE%E3%83%AA%E3%83%95%E3%82%A1%E3%82%AF%E3%82%BF%E3%83%AA%E3%83%B3%E3%82%B0))**

3.  **FE/BE通信構造のリファクタリングによる保守性の向上**
    > FEのコード重複問題を解決するため、自らFEコードを分析し、データ転送ロジックを分離する新たなイベント構造(`room_info`)を設計・実装しました。このリファクタリングを通じて、FE/BE間の結合度を下げ、システム全体の拡張性と保守性を大きく向上させました。
    > * **(技術的な詳細解説: [FEとBEの結合度を下げ、保守性を向上させたWebSocketイベント設計](https://github.com/kushinada2077/NAVER-boostcamp-8-portfolio/wiki/FE%E3%81%A8BE%E3%81%AE%E7%B5%90%E5%90%88%E5%BA%A6%E3%82%92%E4%B8%8B%E3%81%92%E3%80%81%E4%BF%9D%E5%AE%88%E6%80%A7%E3%82%92%E5%90%91%E4%B8%8A%E3%81%95%E3%81%9B%E3%81%9FWebSocket%E3%82%A4%E3%83%99%E3%83%B3%E3%83%88%E8%A8%AD%E8%A8%88))**

# 🎬 主な機能

> **ログインとロビー接続**
> ![bandicam 2023-12-12 20-20-01-282 (1)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/c5b430d1-a375-4760-a38f-8f10586003d5)

> **ルームへの入場**
> ![bandicam 2023-12-12 20-20-01-282 (2)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/4e3145a6-c656-4fd6-be80-82c201c348cd)

> **チャット**
> ![bandicam 2023-12-12 20-20-01-282 (3)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/ce30dc2c-2f23-4238-b61e-039fb8cc1c18)

> **ゲーム開始**
> ![bandicam 2023-12-12 20-20-01-282 (4)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/8a6db8fc-5733-447b-b9c6-44bcd87a102e)

> **コード作成**
> ![bandicam 2023-12-12 20-20-01-282 (5)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/dd791286-964c-4647-84a2-79e39f57f2eb)

> **コードの提出と実行**
> ![bandicam 2023-12-12 20-20-01-282 (6)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/bf5b1d33-32a6-4a08-b3ba-2f4ca1ecc68a)

> **ゲーム終了と結果表示**
> ![bandicam 2023-12-12 20-20-01-282 (7)](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/abccb269-8b4f-4d9f-bfab-c0dfcf14653c)

# ⚙️ 技術スタック

### **FE (フロントエンド)**

![image](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/8690cd01-24cf-48cb-a5df-22a3d00d6c71)

### **BE (バックエンド)**

![image](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/c3f9cf7a-4b00-4eaa-8827-1d3d5d054576)

# ⚒️ アーキテクチャ

![image](https://github.com/boostcampwm2023/web06-CodeClash/assets/77053595/349024e7-af56-4741-a015-03a441bbe8f5)
