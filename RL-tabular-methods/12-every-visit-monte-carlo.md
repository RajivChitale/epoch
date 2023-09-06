### Every Visit Monte Carlo
- The sum of rewards obtained after an occurence of a state in an episode contributes to the value of that state.
- This is averaged over all the occurences of the state. (Repetitions of states are counted in an episode)
- Example episode: A +1 $\rightarrow$ B +4  $\rightarrow$ A +2 $\rightarrow$ C +3
The value of A is [(4+2+3)+(3)]/2 = 6
- This can be efficiently calculated with iterating the sequence in reverse and storing partial sum of reward.