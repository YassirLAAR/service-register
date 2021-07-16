# service-register
Register service, this project contain the configuration files of the following projects:

[company-service](https://github.com/YassirLAAR/company-service "company-service")
[service-config](https://github.com/YassirLAAR/service-config "service-config")

### How to run correctly

#### Create Configuration

Using Git Bash, run the following commands

```sh
$ cd ~
$ cd cloud-conf
$ touche cloud-conf\eureka-service.properties
``` 

Once the file created, Update it with this configuartion:

application.properties:

    server.port=8761
    eureka.client.register-with-eureka=false
    eureka.client.fetch-registry=false
    

Then back to the Git Bash:
```sh
$ cd cloud-conf
$ git add . 
$ git commit -m "Register Config added"
```

#### Running the application

If you're using eclise, go to the class **ServiceRegisterApplication** and run it as JavaApplication

#### Testing the application

In a browser, use this url to see all the apps registered with eureka:
* http://localhost:8761/

![Post Request](https://www.baeldung.com/wp-content/uploads/2016/08/Screenshot_20160819_073151.png)


