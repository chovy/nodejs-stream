NodeJS Stream
=============

An example NodeJS application which uses an event-stream to push notifications to the client side using server side events. Firehose provided by Twitter, Meetup, and Digg.

Install
-------

You may need to install some missing modules with npm. http://npmjs.org/

Once npm is installed, you can checkout the source and install the missing modules:

	$ git clone https://github.com/chovy/nodejs-stream.git
	$ cd ./nodejs-stream
	$ npm install
	$ node stream.js

Browse to your localhost (ie: http://192.168.1.64:8080/) in your web browser.

Configuration
-------------

Configure your twitter account username and password.

Method 1:

	$ export TWITTER_USERNAME='your_username';
	$ export TWITTER_PASSWORD='your_password';

Method 2:

...or edit config.js and set your twitter username password.

	config.twitter_username = process.env.TWITTER_USERNAME || 'my_username';
	config.twitter_password = process.env.TWITTER_PASSWORD || 'my_password';


config.js 
---------

Copy config.sample.js to config.js. Edit config.js and set your port number to listen on and IP address (you can use 'localhost' too).

	config.port = 8080;
	config.address = '192.168.1.64';
