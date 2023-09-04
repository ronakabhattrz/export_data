# ExportData

This gem exports model data into different formats, such as CSV. To achieve so, it uses an export model that handles how the data will be shown

## Installation

```ruby
gem 'export_data'
```

Then, run `bundle install` to install the gem.

## Usage

To use the DataExport::Exporter class, follow these steps:

```ruby
    require 'export_data'
    
    # Prepare data
    data = [
      { id: 1, name: 'John', age: 30 },
      { id: 2, name: 'Alice', age: 25 }
    ]
    
    # Create an instance of the exporter
    exporter = DataExport::Exporter.new
    
    # Export data to a CSV file
    exporter.export_to_csv(data, 'output.csv')
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/ronakabhattrz/export_data. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/ronakabhattrz/export_data/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
