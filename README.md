# 5-qubit-QEC-code-with-random-Pauli-error
This code ouputs a quantum circuit that prepares (not necessarily fault tolerantly) the logical state,|x_L>, for the $5$-qubit code, runs it through a random Pauli error channel, with error rate $p$ , measures syndromes and applies the recovery operations (if needed.) 

We then plot the success of the QEC code vs. the error probability $p$. Finally, we look at an example circuit for $x=1$ and $p=0.1$.

We measure syndromes using the four generators of the stabilizer group of the $5$-qubit code, given by
```math 
\begin{align*}g_1&=\,X Z Z  X  I\\
g_2&=\,I X Z  Z  X\\
g_3&=\,X I X  Z  Z\\
g_4&=\,Z X I  X  Z.
\end{align*}
```
An example of how we decode syndromes can be shown for $X_0$, or, in other words, the case where there is an $X$ error on the $0$th qubit. The operator that represents this error is given by $XIIII$ and then we ask which stabilizers commute with this operator. We can see that $[g_i,XIIII]=0$ for $i=0,1,2,3$ and $[g_4,XIII]\neq 0$ thus our syndrome for $X_0$ is $0001$.


