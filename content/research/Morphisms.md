+++
title = 'A Sane Overview of Homomorphisms in Linear Algebra'
date = 2024-05-14T12:42:10+02:00
draft = true
mathjax = true
toc = true
+++

## Overview
Any Homomorphism is a linear map, which in real terms will be a matrix. Conceptually, homomorphism are gateways between Vector Spaces. Injective, Surjective, Bijective just describe types of mappings/Functions. Depending on the types of mapping (Injective, Surjective, Bijective) there are different kinds of morphisms. 

## Injective, Surjective, Bijective
Consider a mapping $\Phi: V \to W$. Then $\Phi$ is called:

1) Injective: if $\forall \boldsymbol{x}, \boldsymbol{y} \in \mathcal{V}: \Phi(\boldsymbol{x}) = \Phi (\boldsymbol{y}) \Longrightarrow \boldsymbol{x} = \boldsymbol{y}$ 

`Each element of the domain maps to a unique element in the codomain; also known as one-to-one`

2) Surjective: if $\Phi(\mathcal{V})=\mathcal{W}$ 

`all elements in W can be reached from V; Range = Codomain; covering the entire space`

3) Bijective: if it is Injective and Surjective

NOTE: A bijective linear mapping can be undone with the inverse $\Phi^{-1}$. 

## Diving into Morphisms
In concrete terms a linear transformation is always a matrix. In algebraic terms, a linear map or linear transformation can also be called a vector space homomorphism or homomorphism of vector spaces. An invertible homomorphism (where the inverse is also a homomorphism) is called an isomorphism. 

`Think about loss of information; isomorphism means all data points are mapped uniquely, so no information is lost and the structure of the vector space is the same.`  

There are two conditions:
$$
\forall \boldsymbol{x}, \boldsymbol{y} \in V \forall \lambda, \psi \in \mathbb{R}: \Phi(\lambda \boldsymbol{x}+\psi \boldsymbol{y})=\lambda \Phi(\boldsymbol{x})+\psi \Phi(\boldsymbol{y})
$$

- Closure under addition related to associativity 
- Closure under scalar multiplication related to distributivity

`fundamentally it is always important with vector spaces to keep the two properties/closure conditions under consideration.`

## Special Linear Mappings
### Endomorphism
- **Definition**: A linear mapping from a vector space to itself.
- **Form**: $\Phi: V \rightarrow V$ `Note: V to V`
- **Properties**:
  - Preserves vector addition and scalar multiplication.
  - Does not need to be bijective (can be injective, surjective, both, or neither).

### Isomorphism
- **Definition**: A linear mapping between two vector spaces that is bijective.
- **Form**: $\Phi: V \rightarrow W$. `Note: V to W`
- **Properties**:
  - Preserves vector addition and scalar multiplication.
  - **Bijective**: One-to-one (injective) and onto (surjective).
  - Has an inverse mapping $\Phi^{-1}: W \rightarrow V$ that is also linear.

### Automorphism
- **Definition**: A bijective endomorphism.
- **Form**: $\Phi: V \rightarrow V$. `Note: V to V`
- **Properties**:
  - Preserves vector addition and scalar multiplication.
  - **Bijective**: One-to-one (injective) and onto (surjective).
  - Has an inverse mapping $\Phi^{-1}: V \rightarrow V$ that is also linear.
