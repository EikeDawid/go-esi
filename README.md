go-esi
======

ESI implementation for go

Just starting development

ESI:
-----

-  [ESI spec](http://www.w3.org/TR/esi-lang)
-  [Akamai ESI Examples](http://esi-examples.akamai.com/)
  

GO:
-----

-  [goproxy](https://github.com/elazarl/goproxy)
-  [mustache golang](https://github.com/hoisie/mustache)
-  [go html template](http://golang.org/src/pkg/html/template/)
-  [Rob Pike's talk about writing a lexer](http://www.youtube.com/watch?v=HxaD_trXwRE)


Components:
-----
1. Parser for ESI
2. ContentFetcher, parallelised using go routines, results need to be written in order into the stream, handling of 400+, configurable 30X behaviour, capturing of response headers for caching
3. Cache, ideally plugable, initially simple in-memory, memcached
4. integration into goproxy
5. Admin functions
6. Monitoring endpoint ( see revel )

  

