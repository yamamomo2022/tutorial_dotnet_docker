## build

'''bash
docker build -t counter-image -f Dockerfile .
'''

## create container

'''bash
docker create --name core-counter counter-image
'''

## connect

'''bash
docker attach --sig-proxy=false core-counter
^c
'''