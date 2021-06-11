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

