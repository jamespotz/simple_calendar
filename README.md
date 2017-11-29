# simple_calendar
Compatible with Bootstrap 4

## Usage
```ruby
  #helpers/application_helper.rb
  module ApplicationHelper
    require 'calendar'
    def calendar(date = Date.current, disable_date = nil, &block)
      Calendar.new(self, date, disable_date, block).table_compact
    end
  end
```
