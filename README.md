# Hello Rails exercise

> This is an exercise that displays 'Hello World!' to the page by using [Rails](https://guides.rubyonrails.org/) to make sure everything is set up correctly.

<br>

## App created by using the following command:

```
rails new hellorails
```

<br>

## Setup Postgres database:

### 1. Delete this line in the Gemfile:

```
gem 'sqlite3'
```

### 2. Replace it with this code:

```
group :development, :test do
 gem 'sqlite3'
end

group :production do
  gem 'pg'
end
```

### 3. We need to tell the Bundler to ignore the :production group gems in this project

```
bundle config set --local without production
```

### 4. Install all the other gems:

```
bundle install
```

<br>

## Start the app:

```
rails server
```

## Useful links:

- [Ruby](https://ruby-doc.org/)
- [Bundler](https://bundler.io/)
- [RubyGems](https://rubygems.org/)
- [The Odin Project - Installing Rails](https://www.theodinproject.com/lessons/ruby-on-rails-installing-rails)
