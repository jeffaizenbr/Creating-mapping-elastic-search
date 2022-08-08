# Creating-mapping-elastic-search


## creating local CURL

vim /root/curl
```bash
#!/bin/bash

/usr/bin/curl -H "Content-Type: application/json" "$@"
```

## creating content do deploy mapping
```bash
{

        "mappings":{
                        "properties":{
                                        "year":{
                                    "type":"date"
}
}
}
}

```

## Test mapping
```bash
curl -XGET 127.0.0.1:9200/movies2/_mapping?pretty
```



## Insert de FIRST data on indice
vim data2
```bash
{
        "genre" : ["IMAX","Sci-Fi"],
        "title" : "interestellar",
        "year"  : 2014

}
```

entire command to insert first data
```bash
./curl -XPOST 127.0.0.1:9200/movies/_doc/17131713 -d @data2
```

## search your first movie insertion
```bash
curl -XGET 127.0.0.1:9200/movies2/_search?pretty
```


```bash

```


```bash

```


```bash

```


```bash

```


```bash

```


```bash

```


```bash

```


```bash

```
