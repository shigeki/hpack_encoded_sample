hpack_encoded_sample
====================

HTTP/2.0 HPACK-03 encoded sample data.

The original HAR file from
https://github.com/http2/http_samples/blob/master/mnot/yahoo.co.jp.har


Header data is encoded in HPACK-03 with all using one streamfier(request/response) and
is written in JSON format with header_table.

JSON format

````
[{
  'request': {
               'header_set': header set data,
  			   'hpack_encoded_hex': hpack encoded header_set data in hex representation,
			   'header_table': header_table of request after encoded
             },
  'response': {
               'header_set': header set data,
  			   'hpack_encoded_hex': hpack encoded header_set data in hex representation,
			   'header_table': header_table of response after encoded
             },
},
...
]
````
