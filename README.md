Trigram Search
===============

A quick Ruby class to demo Trigram substring inverted index search on a set of strings provided in a CSV.

It's a proof of concept, but the index generated could be used for high speed text matching, such as in autocompletes, or in search services. You could, for example, dump the indexes to JSON and use them client side.

* http://en.wikipedia.org/wiki/Inverted_index
* http://en.wikipedia.org/wiki/Substring_index
* http://en.wikipedia.org/wiki/N-gram

examples
---------

	cd examples
  	ruby spanish_municipalities.rb

There is a Javascript example which uses the generated search index here: http://tokumine.github.com/trigram_search/

benchmark (n=1000)
---------

  	cd examples
  	ruby benchmark.rb

	      user     system      total        real
	  0.950000   0.010000   0.960000 (  0.959077)

>1ms per search

Note - this code is pretty unoptimised