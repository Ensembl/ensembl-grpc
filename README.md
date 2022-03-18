
# ensembl-grpc

This repo contains proto files of all the ensembl core gRPC services.
>For testing Install the [BloomRPC](https://github.com/bloomrpc/bloomrpc) client, select your protobuf files and start making requests.
---
### For example:

Load metasearch-proto/meta-search-service.proto into BloomRPC and make a request.

Sample request payload:
```
{
   "name_pattern":"homo_sapiens_core_1%",
   "filters":[
      {
         "meta_key":"patch",
         "meta_value":"patch"
      }
   ],
   "servers":[
      "anonymous@ensembldb.ensembl.org:3306",
      "anonymous@asiadb.ensembl.org:3306"
   ]
}
```
