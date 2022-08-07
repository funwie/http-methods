## HTTP Methods Summary Table

Why follow this standard? Simplest answer is "Interoperability"
Interoperability is "the ability of computer systems or software to exchange and make use of information" 
Example: Different browsers retrieve and display the same web page 


| HTTP Method      |   Use |   Idempotent   |  Safe | Cacheable | Request body |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| GET      | Retrieve a resource       |  Yes  | Yes | Yes | No |
| POST   | Create a resource        | No  | No | No | Yes|
| PATCH   | Modify part of existing resource        |  No |  No | No | Yes |
| PUT   | Replace existing resource        |  Yes | No | No | Yes |
| DELETE   | Destroy a resource        |  Yes | No | No | No |
| HEAD   | Retrieve headers only (no body)        |  Yes | Yes | Yes | No |
| OPTIONS   | Retrieve supported HTTP methods        |  Yes | Yes | No | No |
| CONNECT   | Open a tunnel for two-way communications       |  No | No  | No | No |
| TRACE   |  Loop- back of the request message        | Yes  | Yes | No | No |


GET - can retrieve many resources (list of same resource type). Include pagination, filters, and sorting.

POST - can create many resources (in bulk). Saves on making many http requests

