# README
## users
|Column|Type|Options|
|------|----|-------|
|name|string|NOT NULL
|email|string|NOT NULL unique: true
|password|string|NOT NULL unique: true

### Association
bilongs_to:groups
bilongs_to:messages

## groups
|Column|Type|Options|
|------|----|-------|
|name|string||
### Association
belongs_to:users
belongs_to:messseges

## messages
|Column|Type|Options|
|------|----|-------|
|messeges|string|
|image|string|
|||

### Association
belongs_to:

## users_groups
|Column|Type|Options|
|------|----|-------|
|users|string|
|groups|string|

### Association
has_many :user
has_many :user

## users
|Column|Type|Options|
|------|----|-------|
|name|string|
|email|string|

### Association
has_many
has_many


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
