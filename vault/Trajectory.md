An (ordered) sequence of states, actions, and rewards an agent experiences in a [[Markov decision process (MDP)]].

$$[S_0, A_0, R_1, S_1, A_1, R_2...]$$

SAR,SAR...

If the environment has natural terminates states ([[episodic environments]]), then it is natural to split up the trajector into epsiodes (superscript notation):


$$[S^1 _0, A^1_0, R^1_1, S^1_1, A^1_1, R^1_2...S^1_T]$$
$$[S^2 _0, A^2_0, R^2_1, S^2_1, A^2_1, R^2_2...S^2_T]$$