# 5-qubit-QEC-code-with-random-Pauli-error
This code ouputs a quantum circuit that prepares (not necessarily fault tolerantly) the logical state,|x_L>, for the $5$-qubit code, runs it through a random Pauli error channel, with error rate $p$ , measures syndromes and applies the recovery operations (if needed.) 

We then plot the success of the QEC code vs. the error probability $p$. Finally, we look at an example circuit for $x=1$ and $p=0.1$.
