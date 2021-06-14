# orbit-diagrams

Orbit diagrams are a new notation for visualizing function types and their composition. The main change is a simple one: instead of writing a function signature as `a -> b`, the codomain is written on a 3D plate, and the plate is orbited by the domain type, all rendered on a 2D surface in orthographic perspective

Here is the Haskell representation of the type of the ```(.)``` function composition operator:

```haskell
λ> :t (.)

(.) :: (b -> c) -> (a -> b) -> a -> c
```

Here is the same thing in orbit diagrams:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/composition.png" width="400" alt="function composition" />
</p>


One way to narrate these diagrams is to consider the plates as containing types that are "guarded" by the orbiting type, and you need that guard type somewhere in the environment already in order to "unlock" the codomain type.  Once unlocked, that codomain type is now in the environment and can unlock the same type wherever it's found guarding another plate. An important constraint is that a plate type cannot unlock itself even if it matches the guard type

I've sketched out a few ideas already in the files above. The notation and arrangements are mine but the equations and proofs they represent are taken from various sources, which I've listed in [references.md](references.md)

More info to follow as the ideas develop

