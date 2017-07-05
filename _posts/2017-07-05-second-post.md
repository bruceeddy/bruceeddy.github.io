---
layout: post
title: My second post
---

# Are we getting somewhere?

## This is what I'm going to write about

Looking good.  The main points are
 
 1. Point 1
 1. Ooops forgot this one
 1. Another point
 1. Point 3
 1. Point 4


```haskell

-- split takes a list and two indices
-- returns a list of elements between the two indices
split :: (Ord a, Num a, Enum a) => [t] -> a -> a -> [t]
split [] _ _ = []
split xs s e
     | s > e = []
     | otherwise = [ b | (a,b) <- (zip [1..] xs), a >= s, a <= e]

```