# mpi-hpp

This repository contains c++ bindings for OpenMPI, currently 5.0.6.

Note that this is nothing fancy nor impressive. So far, I have just
wrapped some functions and structs in the `mpi` namespace so it
"looks more like" c++. Surprisingly, no up-to-date c++ headers can be
found online for OpenMPI. If you want a truly c++ ideomatic implementation
of MPI, look at [Boost.MPI](https://www.boost.org/doc/libs/1_86_0/doc/html/mpi.html),
however the documentation states that "at present, Boost.MPI supports the majority
of functionality of MPI 1.1" which is quite old since the last MPI version
released is 4.x and I don't know what are they planning to do.

## Current State

Currently I have wrapped about 12% of the header file. I was thinking about
cooler techniques for code generation starting from the header like what they
do in [WebGPI-Cpp](https://github.com/eliemichel/WebGPU-Cpp) but this requires
quite some effort and for the time being, just wrapping the functions
manually works. However, I would like to explore more modern and ideomatic
implementations in the future.

## Contributing

If you are also using this and want to add some functions that I did not
wrap, feel free to do so. Doing everything by hand on my own would be
a lot of effort. I'll personally wrap just what I use and I am happy with that.

## License

This header is distributed with the original LICENSE of the OpenMPI project,
as they require. This should be correct, but In the case It is not just
open an issue.