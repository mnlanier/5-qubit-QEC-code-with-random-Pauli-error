# 5-qubit-QEC-code-with-random-Pauli-error
This code ouputs a quantum circuit that prepares (not necessarily fault tolerantly) the logical state,|x_L>, for the $5$-qubit code, runs it through a random Pauli error channel, with error rate $p$ , measures syndromes and applies the recovery operations (if needed.) 

We then plot the success of the QEC code vs. the error probability $p$. Finally, we look at an example circuit for $x=1$ and $p=0.1$.

We measure syndromes using the four generators of the stabilizer group of the $5$-qubit code, given by
```math 
\begin{align*}
g_1&=X\otimes Z\otimes Z \otimes X \otimes I\\
g_2&=\,I\otimes X\otimes Z \otimes Z \otimes X\\
g_3&=\,X\otimes I\otimes X \otimes Z \otimes Z\\
g_4&=\,Z\otimes X\otimes I \otimes X \otimes Z
\end{align*}
```

