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
|content|string|null: false
|image|string|null: false
|user_id|string|null: false
|groups|string|null: false

### Association
belongs_to:groups
belongs_to:users

## users_groups
|Column|Type|Options|
|------|----|-------|
|users_id|integer|null: false
|groups_id|integer|null: false

### Association
belongs_to:users
belongs_to:groups





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
