# cppnd-openstreetmap-route-planner
# C++ Project - OpenStreetMap Route Planner

### Dependencies
- cairo
- graphicsmagick
- io2d

It is probably easier to use the Vagrantfile rather than installing the dependencies manually.

```
vagrant up
vagrant ssh
cd /vagrant
```

### Build
```
mkdir build
cd build
cmake ../
make
```

### Run
The name of the binary file will match the directory you build from.
So, if running from /vagrant:
```
../bin/vagrant -f ../map.osm
```

## Testing

For exercises that have unit tests, the project must be built with the approprate test cpp file. This can be done by using `cmake_tests` instead of `cmake`. For example, from the build directory:
```
cmake_tests ..
make
```
Those commands will build the code with the appropriate tests exercise. The tests can then be run from the `build` directory as follows:
```
../bin/test
```
Not all exercises have tests. The table is given below with the complete list of exercises with tests for reference:

| Exercise Name               | 
|-----------------------------|
| The RouteModel Class        |
| The Node Class              |
| Create RouteModel Nodes     |
| Write the Distance Function |
| Create Road to Node Hashmap |
| Write FindNeighbors         |
| Find the Closest Node       |
| Write the A* Search Stub    |
| Finish A* Search            |
