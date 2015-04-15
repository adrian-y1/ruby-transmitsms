ruby-transmitsms
================

Ruby gem to easily access TransmitSMS RESTful APIs

## Installation
```sh
gem install ruby-transmitsms
```

## Installation with `bundler`'s Gemfile
gem "ruby-transmitsms"

## To install the required gems:
```sh
$ ./setup.sh
```

## To run  the tests:
```sh
$ ./runtest.sh
```

## Sample Usage
```ruby
require 'ruby-transmitsms'

# Create new Sms instance
sms = Sms.new("15eg266c832fb23c4d90f01055aef355", "bluebird")

# Send a message
response = sms.send("Testing sending of sms", "455123456")

# Show the result
puts response.to_body.to_s
```
