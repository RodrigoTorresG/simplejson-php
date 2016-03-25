# SimpleJSON #

The main purpose of this is to allow the parsing of JSON encoded strings into PHP native structures, or PHP objects encoding into JSON strings. Primary target for this are mature systems running versions of PHP older than 5.2, which provides this functionality.

The functions are confirmed to work on PHP as old as 4.1.2.

The functions do not care about character encoding and will do nothing to magically fix character set issues. They'll work with the data as-provided and won't, for example, (un)escape \u0000 or \x00 characters.

Apart from this, the functions (`toJSON`, `fromJSON`) behave as much like the new built in functions ([json\_encode](http://php.net/json_encode), [json\_decode](http://php.net/json_decode)) as possible.