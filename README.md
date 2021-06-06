# Deviseとomniauth-google-oauth2

## omniauth v2
CSRF脆弱性 CVE-2015-9284の対応に伴う変更が入りv2から、
サービスプロバイダーのサービス認可画面へリダイレクトするエンドポイントPOSTのみに変更となりました。

## 解決策
[omniauth-rails_csrf_protection](https://github.com/cookpad/omniauth-rails_csrf_protection)を導入
```
gem "omniauth-rails_csrf_protection"
```