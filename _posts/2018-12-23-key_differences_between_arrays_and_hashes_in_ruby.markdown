---
layout: post
title:      "Key differences between Arrays and Hashes in Ruby"
date:       2018-12-23 23:11:45 -0500
permalink:  key_differences_between_arrays_and_hashes_in_ruby
---


An array is a collection of data. Each element of an array is accessed using an integer which is the index of the element in an array.

**Let's create an array, name**
> name = ["Jordan","James","John"]

Now, if we want to access the elements of an array, we simply do

**name[0]**
>=>will print 'Jordan'

Hash is the collection of key-value pair.In Hash, the value is accessed using the key.

**let's create a hash **

> my_details = {'name' => 'James'}

and if, we want to access the value of hash, we simply do

**my_details['name']**

> =>will print 'James'

A more in-depth explanation about Arrays are ordered, integer-indexed collections of any object. Array indexing starts at 0, as in C or Java. A negative index is assumed to be relative to the end of the array—that is, an index of -1 indicates the last element of the array, -2 is the next to last element in the array, and so on. you can learn more about Arrays [here](http://ruby-doc.org/core-2.5.3/Array.html)

A Hash is a collection of key-value pairs. It is similar to an Array, except that indexing is done via arbitrary keys of any object type, not an integer index. Hashes enumerate their values in the order that the corresponding keys were inserted. Hashes have a default value that is returned when accessing keys that do not exist in the hash. By default, that value is nil. you can learn more about Hashes [here.](http://ruby-doc.org/core-2.5.3/Hash.html)


