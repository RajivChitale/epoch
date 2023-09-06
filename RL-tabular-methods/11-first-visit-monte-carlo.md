### First Visit Monte Carlo
- The sum of rewards obtained after the first occurence of a state in an episode contributes to the value of that state.
- This is averaged over all the episodes in which the state appears. 
- Example episode: A +1 $\rightarrow$ B +4  $\rightarrow$ A +2 $\rightarrow$ C +3
The value of A is (4+2+3)/1 = 9