# NotificationHandler

[![Gem Version](https://badge.fury.io/rb/notification-handler.svg)](https://badge.fury.io/rb/notification-handler) <img src="https://travis-ci.org/jonhue/notifications-rails.svg?branch=master" />

The most powerful (cross-platform) notifications handler & pusher API for Rails.

---

## Table of Contents

* [Installation](#installation)
* [Usage](#usage)
* [Configuration](#configuration)
* [To Do](#to-do)
* [Contributing](#contributing)
    * [Contributors](#contributors)
    * [Semantic versioning](#semantic-versioning)
* [License](#license)

---

## Installation

NotificationHandler works with Rails 5 onwards. You can add it to your `Gemfile` with:

```ruby
gem 'notification-handler'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install notification-handler

If you always want to be up to date fetch the latest from GitHub in your `Gemfile`:

```ruby
gem 'notification-handler', github: 'jonhue/notifications-rails/tree/master/notification-handler'
```

Now run the generator:

    $ rails g notification_handler:install

To wrap things up, migrate the changes to your database:

    $ rails db:migrate

---

## Usage

---

## Configuration

You can configure NotificationHandler by passing a block to `configure`. This can be done in `config/initializers/notification-handler.rb`:

```ruby
NotificationHandler.configure do |config|
    config.default_type = 'notification'
end
```

**`default_type`** Choose your default notification type. Takes a string. Defaults to `'notification'`.

---

## To Do

[Here](https://github.com/jonhue/notifications-rails/projects/2) is the full list of current projects.

To propose your ideas, initiate the discussion by adding a [new issue](https://github.com/jonhue/notifications-rails/issues/new).

---

## Contributing

We hope that you will consider contributing to NotificationHandler. Please read this short overview for some information about how to get started:

[Learn more about contributing to this repository](https://github.com/jonhue/notifications-rails/tree/master/CONTRIBUTING.md), [Code of Conduct](https://github.com/jonhue/notifications-rails/tree/master/CODE_OF_CONDUCT.md)

### Contributors

Give the people some :heart: who are working on this project. See them all at:

https://github.com/jonhue/notifications-rails/graphs/contributors

### Semantic Versioning

NotificationHandler follows Semantic Versioning 2.0 as defined at http://semver.org.

## License

MIT License

Copyright (c) 2017 Jonas Hübotter

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.