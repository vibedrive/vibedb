# vibedb

manage your music library anywhere.


## install 

with [npm](https://www.npmjs.com/)

`npm install -g`


## usage

```
Usage: vibedb 

commands:

  import
  list
  remove
  modify
  move
  update
  write
  stats
  fields
  config
```

## api

```js
var Library = require('vibedb')
```

### Class: Library
represents a database containing songs, which are Item instances.

#### library.items(query, sort)
get Item objects matching the query.

#### library.get(id)
fetch an Item by its ID. Returns None if no match is found.

#### library.add(item)
add the Item object to the library database. 
returns the object’s new id.


### Class: Model
represents an object in the database. 

#### model.keys()
get a list of available keys for objects of this type.

#### model.get(key)

#### model.items()

#### model.load()

#### model.remove()

#### model.set(key)

#### models.update(values)


### Class: Item
represents songs

#### Item.from(path)
#### Item.from(stream)
#### Item.from(buffer)
returns an item instance.

#### item.read(mediaFile)`

#### item.write(mediaFile)


### Class: MediaFile
represents a multimedia file and provides access to its metadata.

#### item.destination(storage)
returns the path in the library directory on a given storage designated for the item.


### Class: Storage
represents a storage medium where a MediaFile can be saved. 



## prior art

- [beets](http://beets.readthedocs.io/)

## see also

- [hyperdb]()
- [ipfs]()
- [omi api spec]()
- [hyperamp]()
