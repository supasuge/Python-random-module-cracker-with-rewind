
# randcrack – Python random module cracker / predictor

Fork of `randcrack`, a python module for cracking/predicting Pythons `random` module. The key difference between this and the original is the ability to "rewind" the state of the PRNG (Mersenne twister under the hood). Once you have >= $624$ 32-bit integer's produced from a seeded PRNG, you can obtain the state and predict the output of the PRNG. 

## Goal
- Rewind state: Find numbers produced at a previous point in time
- Find original state/seed: This is a highly non-trivial task, as the seed you pass to python` `random.seed()` function is then hashed via SHA-512. So, to obtain the original value of the seed, you must brute force this hash.



### Inspiration

The inspiration for forking `randcrack` and making some modification's was solely to help with a recent CTF challenge I was facing in which the flag was the seed, along with a prefix/suffix of 13-1337 random charaters (hex). This made it much easier to brute force with hashcat and custom wordlists... I did not solve the challenge until the event had already completed :(



> Functionality has not been added to master branch yet
> Im busy currently but had enough time to make this README.md file at least...
