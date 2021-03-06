# Terra Amino Decoder

## How to use

* Start rest server
```
$ make install
$ amino-decoder start
```
* Query with rest server
```
curl -X GET http://127.0.0.1:3000/version
curl -X POST http://127.0.0.1:3000/decode/tx  -d '{"amino_encoded_tx": "[amino_encoded_tx]"}'
```

* Directly decode amino encoded tx
```
$ amino-decoder version
$ amino-decoder decode tx [amino-encoded-tx]
```

## How to build
```
# it will create build folder and generate binary for each platform (Windows, Mac, Linux)
$ make  
```

## Use docker
```
$ docker pull quay.io/terra_project/amino-decoder

# it will execute rest server
$ make dockder-run
```
