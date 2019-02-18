# Backbone Relational Model with restorable and diff function:
## Description
This library is a folk version of (Backbone Nested Models)[https://github.com/blittle/backbone-nested-models] by Bret Little, which is to support some additional features as follows:
- An Backbone Model or Backbone Collection can be restored to original state (value).
- Get only changed properties of an Backbone Model or Backbone Collection which is useful to optimize the payload size.

## Usage:

1. Extending Backbone.RelationalModel or RelationalCollection as you need.

```
let model = _.extend({}, Backbone.RelationalModel.prototype, {
    //...
});

```

```
let collection = _.extend({}, Backbone.RelationalCollection.prototype, {
    //...
});
```
2.  Initialization 

```
md.Contacts = md.AddressBook.extend({
    intialize: function(){
        this.relations = {
            {key} : {type}
        };
    }
});
```
[key] : the property of the model   
[type] : the corresponding type assigned to the property


## How to run test

```
$ npm test
```

```
$ npm run test-report
```

Test report is generated in ./test-report.html   
Test coverage report is generated in ./coverage/lcov-report/index.html

## License

(The MIT License)

Copyright (c) 2012 Bret Little

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/blittle/backbone-nested/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

