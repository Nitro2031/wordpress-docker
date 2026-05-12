# wordpress-docker
NginxとMariaDBでWordPressを構築するためのDocker Composeファイルです。

## 使い方
1. このリポジトリをクローンします。
```bash
git clone https://github.com/yourusername/wordpress-docker.git
```
2. クローンしたディレクトリに移動します。
```bash
cd wordpress-docker
```
3. Docker Composeを使用してコンテナを起動します。
```bash
docker-compose up -d
```
4. ブラウザで `http://localhost` にアクセスして、WordPressのセットアップを完了します。
## コンテナ構成
- **nginx**: Nginxウェブサーバー。WordPressのリクエストを処理します。
- **mariadb**: MariaDBデータベースサーバー。WordPressのデータを保存します。
- **wordpress**: WordPressアプリケーション。NginxとMariaDBに接続して動作します。
## 環境変数
- `WORDPRESS_DB_HOST`: データベースホスト（例: `mariadb`）
- `WORDPRESS_DB_USER`: データベースユーザー（例: `wordpress`）
- `WORDPRESS_DB_PASSWORD`: データベースパスワード（例: `wordpress`）
- `WORDPRESS_DB_NAME`: データベース名（例: `wordpress`）
## 注意事項
- データベースのパスワードはセキュリティ上の理由から、実際の運用環境では強力なパスワードを使用してください。
- コンテナを停止するには、以下のコマンドを使用します。
```bash
docker-compose down
```
- データを永続化するために、必要に応じてボリュームを設定してください。
## ライセンス
このプロジェクトはMITライセンスの下で公開されています。詳細はLICENSEファイルを参照してください。
## 貢献
このプロジェクトへの貢献は歓迎します。バグの報告や機能の提案がある場合は、GitHubのIssueを使用してください。また、プルリクエストも歓迎します。
## 作者
- [Your Name](https://github.com/yourusername)
## 参考資料
- [Docker Compose Documentation](https://docs.docker.com/compose/)
- [WordPress Docker Image](https://hub.docker.com/_/wordpress)
- [Nginx Docker Image](https://hub.docker.com/_/nginx)
- [MariaDB Docker Image](https://hub.docker.com/_/mariadb)
## 更新履歴
- 2024-06-01: 初版作成
- 2024-06-15: ドキュメントの更新と改善
- 2024-06-30: セキュリティに関する注意事項の追加
## お問い合わせ
質問やサポートが必要な場合は、[GitHub Issues](https://github.com/yourusername/wordpress-docker/issues) までお問い合わせください。
## 貢献者
- [Contributor 1](https://github.com/contributor1)
- [Contributor 2](https://github.com/contributor2)
- [Contributor 3](https://github.com/contributor3)
## 免責事項
このプロジェクトは「現状のまま」提供されており、明示的または暗示的な保証はありません。プロジェクトの使用に関連するいかなる損害についても、作者は責任を負いません。
## ソースコード
このプロジェクトのソースコードは、[GitHubリポジトリ](https://github.com/yourusername/wordpress-docker) にあります。
## コントリビューションガイドライン
1. フォークしてクローンします。
2. 新しいブランチを作成します。
```bash
git checkout -b feature/your-feature-name
```
3. 変更をコミットします。
```bash
git commit -m "Add your feature description"
```
4. ブランチをプッシュします。
```bash
git push origin feature/your-feature-name
```
5. プルリクエストを作成します。
## コードスタイル
- コードは一貫したスタイルで書いてください。
- コメントを適切に使用して、コードの意図を説明してください。
- 不要なコードやコメントは削除してください。
## テスト
- 変更を加える前に、既存の機能が正常に動作することを確認してください。
- 可能な限り、ユニットテストや統合テストを追加してください。
