# orbit-diagrams

Orbit diagrams are a new notation for visualizing function types and their composition. The main change is a simple one: instead of writing a function signature as `a -> b`, the codomain `b` is written on a 3D plate, and the plate is orbited by the domain type `a`, all rendered on a 2D surface in orthographic perspective

Here is the Haskell representation of the type of the ```(.)``` function composition operator:

```haskell
λ> :t (.)

(.) :: (b -> c) -> (a -> b) -> a -> c
```

Here is the same thing as an orbit diagram:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/composition.png" width="400" alt="function composition" />
</p>


One way to narrate these diagrams is to consider the plates as containing types that are "guarded" by the orbiting type, and you need that guard type somewhere in the environment already in order to "unlock" the codomain type.  Once unlocked, that codomain type is now in the environment and can unlock the same type wherever it's found guarding another plate. An important constraint is that a plate type cannot unlock itself even if it matches the guard type


### μ for `State s`

Here is the **μ** (`join`) instance for the `State s` monad:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/state-s-%CE%BC.jpg" width="500" alt="join for State s" />
</p>


### Functors and Yoneda

Functor instances for `State s` and `Store s`:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/fmap-state-s-store-s.png" width="500" alt="fmap for State s, Store s" />
</p>

Here is `fmap` generally, and the Yoneda Lemma:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/yoneda.png" width="500" alt="fmap and yoneda" />
</p>


### Function from s

The functor and monad instances for `s ->` are elegantly rendered in orbit diagram notation.  Here is the functor instance of `s ->`, and both `bind` and `join` implementations of the `s ->` monad:

<p align="center">
  <img src="https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/function-from-s-functor-monad.png" width="500" alt="functor/monad for s->" />
</p>


### Misc

I've sketched out a few more ideas below (the above images are included here as well):

  - [Function composition](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/composition.png)
  - [Monad instance (`bind`) for continuation passing functor](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/continuation-passing-style-monad-bind.png)
  - [`fmap` for continuation passing functor](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/continuation-passing-style.png)
  - [`fmap` for `State s`, `Store s`](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/fmap-state-s-store-s.png)
  - [`fmap`, `bind`, `join` for `s ->`](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/function-from-s-functor-monad.png)
  - [`join` for `State s`](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/state-s-%CE%BC.jpg)
  - [Yoneda Lemma](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/yoneda.png)

**Lenses:**

  - [Concrete symmetric lenses](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/profunctors-symmetric-lens.png) (derivation by [Boisseau/Gibbons](https://dl.acm.org/doi/10.1145/3236779))
  - [Concrete grates](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/concrete-grate.png)

**Logic:**

  - [**B = S(KS)K** in combinator logic](https://raw.githubusercontent.com/jasonincanada/orbit-diagrams/main/diagrams/sksk-equals-b.png)


## References

The orbit diagrams notation and arrangements are my ideas but the equations and proofs they represent are from various sources. I've listed them in [references.md](references.md)

