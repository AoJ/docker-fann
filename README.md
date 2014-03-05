# Docker fann

- prepared node.js [wrapper](https://github.com/rlidwka/node-fann) for [fann](http://leenissen.dk/fann/wp/)

## Usage

### run script
pipe a node.js script to docker run

    curl -s https://raw.github.com/AoJ/docker-fann/master/examples/xor.js | docker run -i aooj/fann:1.0 node

result

    xor test (0,0) ->  [ 0.01083364801871781 ]
    xor test (1,0) ->  [ 1 ]
    xor test (0,1) ->  [ 1 ]
    xor test (1,1) ->  [ 0.00610451416487365 ]
    Max epochs   100000. Desired error: 0.0000100000.
    Epochs            1. Current error: 0.2500621378. Bit fail 4.
    Epochs           63. Current error: 0.0000096349. Bit fail 0.

## Contributing

### buil
    git clone https://github.com/AoJ/docker-redis.git
    make build
    
### and start it
    make run

### or build, start and attach
    make debug

    
## Changelog
- 1.0 first realese
