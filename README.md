# docker-parity-nginx

Simple docker-compose to launch a contained parity/nginx enviroment.

The main purpose of this project is to create an easy and fast way to launch a (secure) parity instance with RPC capabilities.

JSON-RPC-APIs enabled by default are: `eth,net,parity,parity_pubsub,pubsub,rpc,shh,shh_pubsub,traces,web3`

## Usage

First, find and replace `{{your_address}}` in the project with your IP / domain. This can be done easily with:

```bash
grep -lR "{{ your_address }}" . | xargs sed -i 's/{{ your_address }}/YOUR-ADDRESS/g'
```

Then, launch the docker-compose:

```bash
docker-compose up --build -d
```
