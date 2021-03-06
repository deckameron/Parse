# Parse Android Module

## Description

Appcelerator Titanium module for the Parse SDK. This module currently only support Android Push Notifications

## Usage

### Get it [![gitTio](http://gitt.io/badge.png)](http://gitt.io/component/eu.rebelcorp.parse)
Download the latest distribution ZIP-file and consult the [Titanium Documentation](http://docs.appcelerator.com/titanium/latest/#!/guide/Using_a_Module) on how install it, or simply use the [gitTio CLI](http://gitt.io/cli):

`$ gittio install eu.rebelcorp.parse`

### Example

Put the following code in your app.js (or alloy.js if you are using Alloy) to enable the module.

```javascript
	var Parse = require('eu.rebelcorp.parse');
	Parse.start('<PARSE-APPLICATION-ID>', '<PARSE-CLIENT-ID>');
```

To enable Android Push Notifications

```javascript
    Parse.enablePush();
```

Subscribe of unsubscribe to Parse Channels

```javascript
    Parse.subscribeChannel('user_123');
    Parse.unsubscribeChannel('user_123');
```


## Known Issues

* Not all of the API is exposed at the moment
* Incoming Push Notifications are not exposed when clicked upon


## Changes

**0.1**
- Initial release supporting Android push notifications

## Author

**Timan Rebel**  
twitter: @timanrebel  


## License

The MIT License (MIT)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
