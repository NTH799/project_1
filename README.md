# Large Scale Data Processing: Project 1
## Nicholas Hillis


k | total time of elapsed (s) | number of trials | xS | hash value 
------------| ------------|------------|------------|------------
2 | 10 | 300 | `654465587this_is_a_bitcoin_block_of_68596795` | `00b1d358adf11e726e0538fe4295a15142d616b1fc98df6a9d593d855b97445f`
3 | 11 | 10000 |`1078520280this_is_a_bitcoin_block_of_68596795` | `000f828b69eaffe03e8739d8251bd5858dd16329f9d50a5da02a35176985cbd9`
4 | 12 | 50000 | `858960170this_is_a_bitcoin_block_of_68596795` | `0000e8c7c897b8ecb6c246000e6a5c037572bbf72d0f5a01e646dd768010d86e`
5 | 20 | 1500000 | `1538752746this_is_a_bitcoin_block_of_68596795` | `000000174cefdcccae98dc9fb1b21423b0abcff62b24f10d7dc47ba65457854f`
6 | 127 | 30000000 | `1518978412this_is_a_bitcoin_block_of_68596795` | `000000c86ae1faece07aa5a68c81f5e0c61b25914c07131016435a0b3dada637`


### 2. Run the program on GCP to solve the case k = 7.
k | total time of elapsed (s) | number of trials | xS | hash value 
------------| ------------|------------|------------|------------
7 | 981|250000000|`1150543878this_is_a_bitcoin_block_of_68596795`|`00000003cf71177ef9010a12d5b44ec3bf3b4a090351112cd09f2121c9dc12f5`

*Cluster Configuration*: 
My cluster is just the default settings with one master node and 2 workers. Each has 15 GB of memory

### 3. If we change line 58 to read iter.map(x=>nonce) it changes the code so it is no longer randomized. There should be
not much of a difference between this and upon testing a few trials they appear to be the same as the ones in part 1.  
