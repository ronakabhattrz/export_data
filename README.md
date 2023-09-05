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
# Define a sample class that simulates an object to export
class SampleObject
  attr_accessor :name, :age

  def initialize(name, age)
    @name = name
    @age = age
  end

  # Define a method to get attributes as a hash
  def attributes
    { 'name' => name, 'age' => age }
  end
end

# Create an array of sample objects
sample_objects = [
  SampleObject.new('Alice', 25),
  SampleObject.new('Bob', 30)
]

# Test exporting the objects to a CSV file
DataExport::Exporter.export_to_csv(sample_objects, 'sample.csv')
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and the created tag, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/ronakabhattrz/export_data. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [code of conduct](https://github.com/ronakabhattrz/export_data/blob/master/CODE_OF_CONDUCT.md).

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).