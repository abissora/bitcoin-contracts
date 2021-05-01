This is the readme.md 


### Downloading the Code ###

To download this code, run 

```$ git clone https://github.com/abissora/bitcoin-contracts ```

cd bitcoin-contracts


### Web Server ###

we're using express (handlers.js)

To access the routes using curl:

```curl -get 'http://localhost:8080/transfer```

 - load a file of accounts
 - run the distribution
 - run distro via handler (post)
 - do some fun crypto


### Docker Containers 

To run a docker container, you need to do the following steps:

#### Build it

To build the docker container:

```docker build -t image4 .```

### run it

sudo docker run -p 41690:8090 --name nci11 -d image4

#### Interact with it

**View docker images:** ```docker image ls```

**View running docker containers**: ``` docker ps```

### POST Requests

To post a request, passing in data:

```curl -XPOST http://localhost:8090/distribute -H 'content-type: application/json' -d '{"addresses": ["0x9b14eeE99808BaB2a4C6492D37B4D771F75b7631", "0xe8a43eFC2CE385AbA7465101262b03B0d2489c43", "0x9ca3208d90Ce19f42F2e5FC435ADA5922cB34989","0x1F4aB29bDe4fb3b29d40577c55a7Ae7c1F973351","0x22aF8cf4dE24Cbb09D5D6DA6c6989E0e5315078a","0xFcCE91F39E2C001ED59204A9f321Ce741975E7dd","0x7A768244C32fB024B254acFbE2dFF59919b63898","0x754c68d82DF83699aD2179927c3F9312FF5590e7","0x40581B22EA850D3eC905A4D21f860A489b625d20","0x3f4D34336a1357a19BeBb824166Ac12FAC5676B3"]}'```

```curl -get http://localhost:8090/symbol```

```curl -get http://localhost:8090/transfer```
