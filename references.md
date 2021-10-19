## References

Most concepts in these images are basic category theory and function calculus that I've absorbed over the years from various sources and from working with them in Haskell projects. The following are references to specific places I saw a concept for the first time:


### state-s-store-s-pairing.png

The state/store pairing concept is from page 26 (bottom) of this thesis by Arthur Xavier:

https://arthurxavierx.github.io/ComonadsForUIs.pdf


### continuation-passing-style.png

This is a visual representation of the example given at the bottom of the following comment by Joseph Sible-Reinstate Monica:

https://stackoverflow.com/questions/59122852/how-to-write-functor-instance-of-continuation-monad/59123077#59123077


### continuation-passing-style-monad-bind.png

This is the monad instance, using the `bind` method, of the continuation-passing functor, from page 1 of this paper:

* Ralf Hinze. 2012. Kan Extensions for Program Optimisation <i>Or</i>: Art and Dan Explain an Old Trick. In <i>Proceedings of the 11th international conference on Mathematics of Program Construction</i> (<i>MPC'12</i>). Springer-Verlag, Berlin, Heidelberg, 324–362. https://doi.org/10.1007/978-3-642-31113-0_16

Direct link: https://www.cs.ox.ac.uk/ralf.hinze/Kan.pdf


### profunctors-symmetric-lens.png

The symmetric representation of concrete lenses and its derivation is from pg 84:17 of:

* Guillaume Boisseau and Jeremy Gibbons. 2018. What You Needa Know about Yoneda: Profunctor Optics and the Yoneda Lemma (Functional Pearl). Proc. ACM Program. Lang. 2, ICFP, Article 84 (September 2018), 27 pages.  https://doi.org/10.1145/3236779

Direct link: https://www.cs.ox.ac.uk/jeremy.gibbons/publications/proyo.pdf


### concrete-grate.png

This is the `zipWith3Grate` function from pg 84:23 of the prior reference


### sksk-equals-b.png

This shows how the [**B** combinator](https://en.wikipedia.org/wiki/B,_C,_K,_W_system) can be derived from the [**SKI** combinators](https://en.wikipedia.org/wiki/SKI_combinator_calculus), in particular **B = S(KS)K**, found on Wikipedia [here](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_correspondence#The_composition_combinator_seen_as_a_proof_of_(%CE%B2_%E2%86%92_%CE%B1)_%E2%86%92_(%CE%B3_%E2%86%92_%CE%B2)_%E2%86%92_%CE%B3_%E2%86%92_%CE%B1_in_Hilbert-style_logic)


### jra-to-kra.png

The first row is the `overline` function from p. 2 of the following paper.  The second row denotes that `J r` and `K r` are both functors

* Martín Escardó and Paulo Oliva. 2010. What sequential games, the tychonoff theorem and the double-negation shift have in common. In Proceedings of the third ACM SIGPLAN workshop on Mathematically structured functional programming (MSFP '10). Association for Computing Machinery, New York, NY, USA, 21–32. DOI: https://doi.org/10.1145/1863597.1863605

### otimes.png

This is the `otimes` function from p. 4 of the prior paper.  It's a bit non-obvious that the function `p` needs to be applied, and twice, with a different pair `(a,b)` each time. At present it needs to be inferred by the reader and it's a bit unclear

### otimes2.png

Same as above but with the `b -> r` lambda functions removed, and the  `(a,b)` argument on the bottom left curried
