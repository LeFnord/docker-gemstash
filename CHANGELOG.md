# Changelog

## 1.5.0

* Upgrade Ruby to v3.1.2.
* Upgrade Bundler to v2.3.13.
* Upgrade Gemstash to v2.1.0.
* Bump activesupport from 5.2.4.4 to 5.2.8.
* Bump concurrent-ruby from 1.1.7 to 1.1.10.
* Bump dalli from 2.7.10 to 2.7.11.
* Bump faraday from 0.15.4 to 0.17.5.
* Bump faraday_middleware from 0.13.1 to 0.14.0.
* Bump i18n from 1.8.5 to 1.10.0.
* Bump minitest from 5.14.2 to 5.15.0.
* Bump multipart-post from 2.0.0 to 2.1.1.
* Bump mysql2 from 0.5.2 to 0.5.4.
* Bump pg from 0.18.4 to 1.3.5.
* Bump puma from 3.12.6 to 4.3.12.
* Bump sequel from 5.19.0 to 5.56.0.
* Bump sinatra from 2.0.5 to 2.2.0.
* Bump sqlite3 from 1.4.1 to 1.4.2.
* Bump tzinfo from 1.2.7 to 1.2.9.

## 1.4.1

* Bump puma from 3.12.1 to 3.12.6.
* Bump rack from 2.0.7 to 2.2.3.
* Bump activesupport from 5.2.3 to 5.2.4.4.

## 1.4.0

* Always specify the config file in the command and always run as gemstash user.

## 1.3.0

* Add `GEMSTASH_PROTECTED_FETCH` configuration option to enable protected
  fetches which is disabled by default.

## 1.2.0

* Upgrade Ruby to v2.6.3.
* Upgrade Gemstash to v2.0.0.

## 1.1.0

### 2018-02-23

* Upgrade to Ruby 2.5.0.
* Default `:puma_threads` to 16 if not specified by the `GEMSTASH_PUMA_THREADS` environment variable.

### 2017-08-10

* Package gemstash v1.1.0.
* Install system libraries for all database drivers i.e. postgresql, mysql2.
* Define Ruby dependencies via `Gemfile.lock`.
* Run gemstash as `gemstash` user instead of `root`.
* Add dynamic configuration with MySQL, PostgreSQL and SQLite support.
