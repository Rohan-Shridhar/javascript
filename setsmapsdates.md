# Sets
A set is a collection of values, such that no value appears more than
once and the order in which the values occur in the set is irrelevant.

Operations are:
* new Set(iter) — Creates and returns a new set containing the values
in the iterable object iter (often an array). To create an empty set, omit
iter.
If iter is a map, the result is a set of [key, value] arrays.

* set.has(value) — Tests if value is a member of set.

* set.add(value) — Adds value to set if it is not already present, and
returns set.

* set.delete(value) — If value is in set, it is deleted. delete does not
return set; it returns true if value was in set, and false otherwise.

* set.clear() — Removes all values from set and returns undefined.

* set.size — Returns the number of elements in set.

# Maps
Maps are lookup tables. Each entry in a map consists of a key-value pair.
Keys must be unique, but the same value may occur multiple times.

Operations are:
* new Map() — Creates and returns a new, empty map.

* new Map(array_or_set) — The array_or_set must consist of [key,
value] arrays; this returns a map with those keys and values.

* map.has(key) — Tests if map contains the given key.

* map.set(key, value) — Sets or changes the value associated with
key to value and returns the modified map.

* map.get(key) — Returns the value associated with key, or undefined
if key is not in the map.

* map.delete(key) — Removes key and its associated value from

* map. Returns true if map was changed, false if key wasn’t found in
map.

* map.clear() — Removes all values from map and returns
undefined.

* map.size — Returns the number of key-value pairs in map.

# Dates
JavaScript has a Date object, which can be created in any of the following
ways:

* new Date() — Returns the current date and time in the browser’s time
zone.

* new Date(ms) — Returns the date that corresponds to the number of
milliseconds since “epoch” (January 1, 1970).

* new Date(year, month, day, hours, minutes, seconds,
milliseconds)
Up to five arguments may be omitted from the right end, for
example, new Date(year, month, day).
You cannot supply just a year, because a single argument will be
taken as milliseconds.
If the year is less than 100, 1900 will be added to it.

* new Date(string) — Converts string into a Date, if possible, and
returns it. The International Standard format is yyyy-mm-dd, but many
other formats are recognized.

Operations are:
* date.getFullYear() and date.setFullYear(year)

* date.setFullYear may also be given month and day arguments.

* date.getMonth() and date.setMonth(n), where n is 0 (January) to 11
(December).

* date.getDate() and date.setDate(n), where n is 1 to 31.

* date.getHours() and date.setHours(n), where n is 0 to 23.

* date.getMinutes() and date.setMinutes(n), where n is 0 to 59.

* date.getSeconds() and date.setSeconds(n), where n is 0 to 59.

* date.getMilliseconds() and date.setMilliseconds(n), where n is
0 to 999.

* date.getTime() and date.setTime(n), where n is milliseconds since
epoch.

* Date.now() also returns milliseconds since epoch but is shorter
than new Date().getTime().

* date.getDay() returns 0 to 6, where 0 means Sunday (regardless of
where you are, and despite ISO 8601 specifying Monday as the first
day of the week).

