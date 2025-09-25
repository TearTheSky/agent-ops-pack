# 🔧 Error Handling Knowledge Base

## 📋 概要

AIエージェントと人間の協働における、実際に発生したエラーとその解決策のナレッジベースです。
実運用で効果が実証された解決手順を体系化しています。

## 🎯 使用方法

### AIエージェント向け
1. **エラー発生時**: エラーメッセージや症状から該当ファイルを特定
2. **解決手順実行**: step-by-step で記載された手順に従う
3. **結果記録**: 解決後は進捗TSVとエビデンス生成を実行

### 人間向け
1. **事前学習**: よくあるエラーパターンの把握
2. **レビュー**: AIが実行した解決策の確認
3. **ナレッジ追加**: 新しいエラーパターンの文書化

## 📂 エラーカテゴリ

### Infrastructure & Terraform
- `provider_version_conflict.yaml` - Google Provider バージョン競合
- `terraform_state_lock.yaml` - Terraform State ロック問題
- `resource_dependency.yaml` - リソース依存関係エラー

### CI/CD Issues  
- `ci_authentication_failure.yaml` - CI認証エラー
- `build_timeout.yaml` - ビルドタイムアウト
- `test_failure_patterns.yaml` - テスト失敗パターン

### Cloud Provider Specific
- `gcp_permission_denied.yaml` - GCP権限エラー
- `azure_resource_registration.yaml` - Azure リソース登録問題
- `aws_service_quota.yaml` - AWS サービスクォータ

### Development Environment
- `git_branch_conflicts.yaml` - Git ブランチ競合
- `dependency_version_mismatch.yaml` - 依存関係バージョン不整合
- `local_environment_setup.yaml` - ローカル環境セットアップ

## 🔍 エラー特定ガイド

### エラーメッセージによる分類
```
"edition" is not expected here
→ provider_version_conflict.yaml

"terraform state lock"
→ terraform_state_lock.yaml

"permission denied"
→ gcp_permission_denied.yaml

"microsoft.insights already exists"
→ azure_resource_registration.yaml
```

### 症状による分類
```
CI が突然失敗し始めた
→ provider_version_conflict.yaml or ci_authentication_failure.yaml

PR作成後にテストが通らない
→ test_failure_patterns.yaml or dependency_version_mismatch.yaml

スクリプト実行で権限エラー
→ gcp_permission_denied.yaml or authentication系
```

## 📈 ナレッジベース拡張

### 新しいエラーパターンの追加
1. **実際のエラー発生**: 新しいパターンを発見
2. **解決策の検証**: 確実に動作する手順を確立
3. **文書化**: テンプレートに従って手順書作成
4. **テスト**: 他のケースでの再現性確認

### 品質基準
- ✅ **再現可能**: 同じ手順で確実に解決
- ✅ **AI実行可能**: 明確で具体的な指示
- ✅ **時短効果**: 従来より効率的
- ✅ **証跡生成**: エビデンス作成まで含む

## 🤖 AI思考パターン最適化

### 直感的なファイル名
```
❌ error_handling_provider_version_conflict.yaml
✅ provider_version_conflict.yaml
```

### カテゴリ別ディレクトリ構造
```
error_handling/
├── infrastructure/
│   ├── provider_version_conflict.yaml
│   └── terraform_state_lock.yaml
├── ci_cd/
│   ├── authentication_failure.yaml
│   └── build_timeout.yaml
└── cloud_provider/
    ├── gcp_permission_denied.yaml
    └── azure_resource_registration.yaml
```

### 検索キーワード最適化
- エラーメッセージの重要部分をファイル名に含める
- 症状から逆引きできるメタデータ付与
- 関連エラーへのクロスリファレンス

## 🔄 継続的改善

### 定期レビュー
- 月次: 新しいエラーパターンの追加
- 四半期: 解決手順の効率性見直し
- 年次: カテゴリ構造の再編成

### 効果測定
- エラー解決時間の短縮率
- 再発防止効果
- AIエージェントの成功率向上

---

**このナレッジベースは実際の運用経験に基づいて継続的に拡張されます。**
