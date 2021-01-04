# テーブル設計

## users テーブル

| Column     | Type   | Options     |
| ---------- | ------ | ----------- |
| name       | string | null: false |
| email      | string | null: false |
| password   | string | null: false |
| profile    | text   | null: false |
| occupation | text   | null: false|
| position   | text   | null: false |

## prototype テーブル

| Column     | Type   | Options     |
| ---------- | ------ | ----------- |
| title      | string | null: false |
| catch_copy | text   | null: false |
| concept    | text   | null: false |
| user       | text   | ----------- |

## comments テーブル

| Column    | Type          | Options                        |
| --------- | ------------- | ------------------------------ |
| user      | references    | null: false, foreign_key: true |
| text      | text          | ------------------------------ |
| prototype | references    | -------------------------------|