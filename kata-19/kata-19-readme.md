# Kata Nineteen - Word Chains
Write a program that solves word-chain puzzles.

There’s a type of puzzle where the challenge is to build a chain of words, starting with one particular word and ending with another. Successive entries in the chain must all be real words, and each can differ from the previous word by just one letter. For example, you can get from "cat" to "dog" using the following chain.

```
cat
cot
cog
dog
```

The objective of this kata is to write a program that accepts start and end words and, using words from the dictionary, builds a word chain between them. For added programming fun, return the shortest word chain that solves each puzzle. For example, my Powerbook running Ruby can turn "lead" into "gold" in four steps (lead, load, goad, gold), taking about 20 seconds. Turning "ruby" into "code" takes six steps (ruby, rubs, robs, rods, rode, code) and 90 seconds, while turning "code" into "ruby" (again in six steps) takes about an hour. Go figure…

Update: It turns out that my original algorithm was pretty dumb: a better approach greatly speeds up search and makes it symetrical. It now does all the above examples in between 0.5s and 1s.
