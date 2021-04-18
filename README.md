# Docker-IPFS
Simple Go-IPFS setup inside Docker container
___

## About IPFS
[Documentation](docs.ipfs.io)

[GitHub Repository](https://github.com/ipfs/go-ipfs)

## Setup
1. Run `git clone https://github.com/fmedv/docker-ipfs`.
1. Rename `.env-example` to `.env`.
1. Run `docker-compose pull`.
1. Run `docker-compose up -d`.
1. Open browser and go to URL `${APP_HOST}:${IPFS_API_PORT}/webui`

## Important CLI commands
* Run `ipfs add ${IPFS_FILE_PATH}/FILE_NAME` to add an object and get unique content identifier (CID).
* Run `ipfs pin add CID` to ensure that object is stored indefinitely and not just cashed.
* Run `ipfs pin rm CID` to unpin an object.
* Run `ipfs cat CID` to print the content of the corresponding object.
