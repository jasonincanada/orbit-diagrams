# orbit-diagrams

Orbit diagrams are a new notation for visualizing function types and their composition. The main change is a simple one: instead of writing a function signature as `C -> D`, with an arrow separating the domain type from codomain type, the codomain is written on a 3D plate (I picture a glass microscope slide), which is orbited by the domain type, all rendered on a 2D surface in orthographic perspective

A simple way to narrate these depictions is to consider the plates as containing types that are "guarded" by the orbiting type, and you need that guard type somewhere in the environment already in order to "unlock" the codomain type.  Once unlocked, that codomain type is now in the environment and can unlock the same type wherever it's found guarding another plate. An important constraint is that a plate type cannot unlock itself even if it matches the guard type

I've sketched out a few ideas already in the files above. The notation and arrangements are mine but the equations and proofs they represent are taken from various sources, which I've listed in [references.md](references.md)

More info to follow as the ideas develop

