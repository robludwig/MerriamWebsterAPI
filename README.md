MerriamWebsterAPI
=================

A demo Python implementation of the Merriam-Webster Inc. API for use in Python applications. For more information see the offical
[Merriam-Webster page](http://www.dictionaryapi.com/) for the API. 

As the API only allows developers to have keys to 2 services, I was only able to implement parsers for the ones I was interested in,
namely the Collegiate® Thesaurus API and the Collegiate® Dictionary. If you're interested in more, find a way to hook me up with keys to other
products.

As it stands, you can get a quick definition of a word by doing

```
import mwapi

APIKEY = 'this is the key i got from MW'
dictionary = mwapi.DictionaryAPI(APIKEY)
definition = dictionary.get_definition(word)
```


The api object will cache results for you as you make queries, so you don't have to worry about running up against your limit
for querying for the same result multiple times, or different properties of the same result.

I don't own trademarks for any of this stuff. If you choose to use this library, you should to follow the API's [branding guidelines](http://www.dictionaryapi.com/info/branding-guidelines.htm) and all appropriate licensing stuff.
