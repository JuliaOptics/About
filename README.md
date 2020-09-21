# About

JuliaOptics is an organization to house a suite of libraries for physical optics in Julia.  This suite has particular goals from the outset:

- To respect the prior art that exists in the enumerable physical optics codes written in matlab, python, and so on and learn from their API design.

- To provide a minimal API that is easy to learn with a reasonable balance between explicit and "fluent" design.

- To enable truly next generation computation in optics through automatic differentiation and other areas of significant development in Julia.

This provides a set of guiding performance marks:

- To be more than (5x required, 100x desired) faster than prysm, the fastest public physical optics code.

- To freely support computation on CPU or GPU

- To force as few allocations as possible, keeping GC time below 15% overall.

The goal at the outset is not to have all features, but to specialize in computational physical optics with emphasis on propagation from pupil to PSF or vice-versa, and between planes.  A numerical model of propagation through a coronagraph (two plane to plane, then pupil => PSF => pupil => PSF) will demonstrate the performance efficacy (or lack thereof) of Julia for this domain.
