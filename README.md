# README
## users
|Column|Type|Options|
|------|----|-------|
|name|string|null: false
|email|string|null: false
|password|string|null: false

### Association
has_many :users_groups
has_many :groupss, through: :users_groups
has_many :messeges

## groups
|Column|Type|Options|
|------|----|-------|
|name|string|null: false

### Association
has_many :users_groups
has_many :users, through: :users_groups
has_many :messeges

## messages
|Column|Type|Options|
|------|----|-------|
|content|text|
|image|text|
|user_id|integer|null: false, foreign_key: true
|group_id|integer|null: false, foreign_key: true

### Association
belongs_to:group
belongs_to:user

## users_groups
|Column|Type|Options|
|------|----|-------|
|user_id|integer|null: false, foreign_key: true
|group_id|integer|null: false, foreign_key: true

### Association
belongs_to:user
belongs_to:group





This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
