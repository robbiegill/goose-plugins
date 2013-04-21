# goose-plugins

Simple Plugins for Mongoose (v0.0.1)

## How to use

Simply use the `plugin` method of Mongoose schemas to add properties

### Created Timestamp [`ts_created`]

Set the timestamp when `myDoc` is created as property `myDoc.ts_created`

    var Schema = require('mongoose').Schema;
    var goose = require('goose-plugins');

    var mySchema = new Schema();
    mySchema.plugin(goose.ts_created);
  
  
### Modified Timestamp [`ts_modified`]

Update `myDoc.ts_modified` each time the document is saved.

    var mongoose = require('mongoose').Schema;
    var goose = require('goose-plugins');

    var mySchema = new Schema();
    mySchema.plugin(goose.ts_modified);
    
## License

OSI: The BSD License, FSF: The Modified BSD License
