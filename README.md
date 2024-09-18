# ObsoleteIdentityMatrix

NOTE: This package is archived. It was never registered. This repo name has been changed
from `IdentityMatrix` to `ObsoleteIdentityMatrix.jl`.
A new (as of now unregistered) pacakge with
similar goals is [IdentityMatrix.jl](https://github.com/jlapeyre/IdentityMatrix.jl).

NOTE: This package is being canibalized; Pieces moved to `FillArrays.jl` and `LinearAlgebra`.
If you don't have all these in sync,
you make get warnings or errors about redefined methods.
But, the master branches of `IdentityMatrix.jl` and `FillArrays.jl` will be kept in sync.

This package implements several methods specialized for types `Diagonal`,
`FillArrays.Fill`, and `FillArrays.Eye`.
They are more efficient, often much more, than the fallback methods.

The methods are more-or-less drop-in replacements.

To use, load the module
```julia
using FillArrays
using IdentityMatrix
```

* `iterate`

* `copy`, `Matrix`

* `kron(a, b)`, where either or both of `a` and `b` is an identity matrix or a `Diagonal` matrix.

* `IM::Idents / A::AbstractMatrix`

* `A::AbstractMatrix / IM::Idents`

* `IM::Idents \ A::AbstractMatrix`

* `A::AbstractMatrix \ IM::Idents`

* `IM::Idents * A::AbstractMatrix`

* `A::AbstractMatrix * IM::Idents`

*  Matrix operations with `UniformScaling`

* `^(IM::Idents, p::Integer)`

* `eigen`, `eigvecs`, `eigvals`

* `isposdef`, `imag`

* `diag`, `first`, `last`, `minimum`, `maximum`, `extrema`, `any`, `all`, `sum`, `prod`

* `norm`, `opnorm`

* `permutedims`, `triu` `triu!`, `tril`,  `tril`, `inv`

* `det`, `logdet`

<!--  LocalWords:  IdentityMatrix Codecov FillArrays julia idmat fallbacks kron
 -->
<!--  LocalWords:  UniformScaling eigen eigvecs eigvals isposdef imag diag triu
 -->
<!--  LocalWords:  extrema opnorm permutedims tril inv det logdet
 -->
