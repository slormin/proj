# proj

mytheresa Promotions Test

this project needs to be installed in a Apache local server (XAMPP can be used for instance).

Files needs to be copied within a subdirectory of /htdocs, for instance /htdocs/mytheresa

After it, you can either:

1. Open a browser and launch GET request to the following endpoint: http://localhost/mytheresa/products.php

  Examples:
  http://localhost/myTheresa/products.php
  http://localhost/myTheresa/products.php?priceLessThan=72000
  http://localhost/myTheresa/products.php?category=boots
  http://localhost/myTheresa/products.php?priceLessThan=72000&category=boots
  
2. Use php command in a shell window within htdocs/mytheresa:

  php script.php --url=http://localhost/myTheresa/products.php?category=boots
  

The project is splitted in 3 folders:
- Controller: that accept all the requests to the endpoint
- Gateway: in this case the persistence model chosen is a json file fetched from the filesystem, but it could be a coonection to the database where all data would be stored
- Model: with Product and Price data classes (POJO) with private attributes


