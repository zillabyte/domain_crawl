# Easy Domain Crawling

This [Zillabyte Component](http://docs.zillabyte.com/quickstart/faq/#what_are_components) will crawl an entire web domain and return the results as a new dataset. 

You can execute this component from the command line: 

```bash
$ zillabyte execute "domain_crawl" "docs.zillabyte.com"
```

Or, you can stitch this component into your own [Data App](http://docs.zillabyte.com/quickstart/faq/#what_are_apps).

```ruby
app = Zillabyte.app("your_app")
stream = app.source(...)
stream = stream.call_component("domain_crawl")
stream.sink(...)
```

For more information, check out [docs.zillabyte.com](http://docs.zillabyte.com)

[![Powered by Zillabyte](http://www.zillabyte.com/powered_by.png)](http://docs.zillabyte.com/)
