# F00pxScraper

Exports a list of photographers from the various 500px photo streams (popular, editors, fresh, etc.)

You specify which feature list, starting and end pages, # of results per page (max 100) and it will use the API to grab the photos for the feature list, and lookup photographer details for that list and save them to a CSV file.

[future]
- Future options will be to filter by certain categories

## Installation

Add this line to your application's Gemfile:

    gem 'f00px_scraper'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install f00px_scraper

## Usage
```
$ ./bin/500px_scraper_cli
Commands:
  500px_scraper_cli csv k, --key=KEY  # export list of photographers from FEATURE list to csv file
  500px_scraper_cli help [COMMAND]    # Describe available commands or one specific command

$ 500px_scraper_cli --key=<YOUR CONSUMER KEY> 
  This will extract the top 20 photographers from the popular list


  to follow users
  > cat filename.txt | xargs t follow 
 
  to add to list
  > cat filename.txt | xargs t list add <listname>
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
