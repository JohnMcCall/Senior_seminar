# Comments on "Zero Knowledge Compilers"

## High Level

The structure of the paper seems to be appropriate. The pace of the paper is
good except for section surrounding equations (1) and (2). I don't see any
obvious high-level defects at this time.

One confusing aspect of the paper is the usage of "proof" versus "protocol".
If these terms really do mean separate things, then it appears that they are
conflated in various parts of the paper.

## Abstract

The abstract is currently a short outline of the paper -- save that for the
introduction. In the abstract I want to know *what* is discussed, not *how* it
is discussed. By focusing on what is dissussed, some room in the abstract
should be freed up; is there any other red meat we can put in the abstract to
entice readers to actually read the paper?

## 2. Zero knowledge protocols

> An interactive proof system for a set S is an interaction [...]

Since you're introducing interactive proof systems to individuals who may not
be familiar to them, consider mentioning what are the elements of the set `S`.
For example, changing the verbage to "[...] for a set of statements S [...]"
means that the reader is no longer wonder what the set S is until it is
filled in by context.

If space permits, defining what is a probabilistic polynomial-time strategy
may be useful. If I remember correctly I was first formally introduced to that
definition in my cryptography course, so other readers may not have the
appropriate background.

## 2.1 Examples

> First presented in [7] and then restated in [5]
the cave example is the go-to example for learning zero
knowledge protocols.

I believe this sentence could use a comma after "[5]".

> Victor hears about this, and offers to buy the secret from
Peggy

Missing period at the end.

> Before giving Peggy the money Victor wants

A comma after "money" may be useful.

## 3. Compilers

> There are many different types of compilers, single-pass
compilers, multi-pass, load-and-go, debugging compilers, op-
timizing compilers, and many combinations of these. Differ-
ent compilers do different things, [...]

This looks like fluff to me. Eliminate it and start with the function that
compilers perform.

## 5. Zero knowledge compilers

> Due to the subtleties of implementing a zero knowledge
proof they can be diffcult to get correct.

Consider making this sentence more direct by flipping it around: "It is
difficult to correctly implement zero knowledge proofs due to their
subtleties." Additionally, did you mean "protocols" and not "proofs"?

## 5.1 Sigma-protocols

It looks like something is screwed up with equation (1) and (2).

> Also, in both of the above equations linear relations
can be proven implicitly [...]

I'm not following this part at this time.

## 5.2 ZKCrypt

> In the final phase, generation,
the optimized implementation is converted into C and Java
implementations of the protocol.

Random though: Has the correctness of this conversion been proved?

## 5.3 ZKPDL

> Instead, they use the Fiat-Shamir heuristic [...]

What is the Fiat-Shamir heuristic? At least give a citation that the reader can
explore.

## 6.1 Electronic Cash

> Bitcoins are a recent example of an e-cash system.

Mentioning Bitcoin is useful, but the notion that it is an e-cash system can be
debatable depending on the exact definition used.

## 7. Conclusion

> Because they can be increadably complex and take a while to implement

Previously "difficult" was used instead of "take a while to implement".
Consider using the same structure here.
