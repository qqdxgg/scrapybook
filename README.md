Learning Scrapy Book
==========

This book covers the long awaited Scrapy v 1.0 that empowers you to extract useful data from virtually any source with very little effort. It starts off by explaining the fundamentals of Scrapy framework, followed by a thorough description of how to extract data from any source, clean it up, shape it as per your requirement using Python and 3rd party APIs. Next you will be familiarised with the process of storing the scrapped data in databases as well as search engines and performing real time analytics on them with Spark Streaming. By the end of this book, you will perfect the art of scarping data for your applications with ease.

This book is now available on [Amazon](http://amzn.to/1PeQ5O0) and [Packt](https://www.packtpub.com/big-data-and-business-intelligence/learning-scrapy).

## What you will learn

- Understand HTML pages and write XPath to extract the data you need
- Write Scrapy spiders with simple Python and do web crawls
- Push your data into any database, search engine or analytics system
- Configure your spider to download files, images and use proxies
- Create efficient pipelines that shape data in precisely the form you want
- Use Twisted Asynchronous API to process hundreds of items concurrently
- Make your crawler super-fast by learning how to tune Scrapy's performance
- Perform large scale distributed crawls with scrapyd and scrapinghub

See also [the official website](http://scrapybook.com)

## Alternative installation instructions

In some regions, the Vagrant-Docker system takes some time to set-up. This alternative method will help you resolve any issues.

Step 1. Download and add [the Vagrant box](http://scrapybook.com/scrapybook.box) either manually or with something like wget:

```
$ wget http://scrapybook.com/scrapybook.box
$ vagrant box add scrapybook scrapybook.box
```

Notes:
* Downloading (2.8 GB) will likely take a few minutes
* Make sure `scrapybook.box` is on your current directory while doing `vagrant box add`.
* You can check with `vagrant box list` that the box was successfully added.

Step 2. Clone this repo and edit Vagrantfile:

```
$ git clone git@github.com:scalingexcellence/scrapybook.git
```

Edit `Vagrantfile` and replace `"./Vagrantfile.dockerhost"` with `"./Vagrantfile.dockerhost.boxed"`.

That was it! You can start the system as usual with `vagrant up --no-parallel`. There will be no extra downloads and it will take just a few seconds.
