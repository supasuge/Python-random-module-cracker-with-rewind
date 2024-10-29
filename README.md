
# randcrack – Python random module cracker / predictor

**Incomplete project...**

Fork of `randcrack`, a python module for cracking/predicting Pythons `random` module. The key difference between this and the original is the ability to "rewind" the state of the PRNG (Mersenne twister under the hood). Once you have >= $624$ 32-bit integer's produced from a seeded PRNG, you can obtain the state and predict the output of the PRNG. 

## Goal
- Rewind state: Find numbers produced at a previous point in time
- Find original seed used after rewinding state 



### Inspiration

The inspiration for forking `randcrack` and making some modification's was solely to help with a recent CTF challenge I was facing in which the flag was the seed, along with a prefix/suffix of 13-1337 random charaters (hex). 




