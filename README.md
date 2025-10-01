# 民宿予約サイト - Samurai Travel

![Java](https://img.shields.io/badge/Java-21-orange)
![Spring Boot](https://img.shields.io/badge/SpringBoot-3.3-green)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-template-lightgreen)
![Stripe](https://img.shields.io/badge/Stripe-Payment-purple)

## 📖 概要
**Samurai Travel** は、Spring Boot を用い、侍エンジニアの教材をベースに開発した民宿予約アプリケーションです。  
未経験から Web エンジニアを目指す過程で、バックエンド・フロントエンド・DB・外部サービス連携（Stripe）を組み合わせた総合的な開発経験を積むために制作しました。

ユーザーは会員登録を行い、宿泊施設の検索・予約・キャンセル、レビュー投稿、お気に入り登録、クレジットカード決済が可能です。

---

## 🚀 使用技術
- **フロントエンド**
  - HTML / CSS / JavaScript
  - Bootstrap 5
  - Thymeleaf (テンプレートエンジン)

- **バックエンド**
  - Java 21 (Eclipse Temurin)
  - Spring Boot 3.3
  - Spring Security
  - JPA / Hibernate

- **データベース**
  - MySQL (XAMPP / JawsDB Maria for Heroku)

- **外部サービス**
  - Stripe API（決済処理）
  - Mailgun（メール送信）

- **開発環境**
  - Eclipse
  - Maven
  - GitHub / Heroku

---

## ✨ 主な機能
- ユーザー認証
  - 新規会員登録 / ログイン / ログアウト
- 宿泊予約
  - 施設一覧 / 詳細ページ
  - 予約・キャンセル機能
- 決済機能
  - Stripe API によるクレジットカード決済
- レビュー機能
  - 宿泊後にレビュー投稿 / 閲覧
- お気に入り機能
  - 施設のお気に入り登録・解除
- 管理者機能（Admin）
  - 宿泊施設の登録・編集・削除

---

## 🛠️ 環境構築方法
1. リポジトリをクローン
   ```bash
   git clone https://github.com/gororian0318/samuraitravel.git
   cd samuraitravel
   
2. application.properties を設定（例）
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/samuraitravel
   spring.datasource.username=root
   spring.datasource.password=password
   spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

   stripe.api-key=sk_test_********
   stripe.success-url=http://localhost:8080/reservations?reserved
   stripe.cancel-url=http://localhost:8080/reservations?canceled

3. DBマイグレーションを実行
   ```bash
   ./mvnw spring-boot:run

4. ブラウザでアクセス
   ```arduino
   http://localhost:8080

🎯 今後の改善点
　レスポンシブデザインの強化

---

## 👤 制作者
門田 滉暉 (Kadota Hiroki)

31歳 / Webエンジニア転職活動中

学習期間：2025年4月〜9月

GitHub: gororian0318

