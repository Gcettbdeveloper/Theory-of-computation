# Introduction

Automata theory (also known as Theory Of Computation) is a theoretical branch of Computer Science and Mathematics, which mainly deals with the logic of computation with respect to simple machines, referred to as automata. 

Automata* enables scientists to understand how machines compute the functions and solve problems. The main motivation behind developing Automata Theory was to develop methods to describe and analyze the dynamic behavior of discrete systems. 

Automata originated from the word “Automaton” which is closely related to “Automation”


# 1. Deterministic Finite Automata (DFA):

DFA consists of 5 tuples {Q, Σ, q, F, δ}. 
- Q : set of all states.
- Σ : set of input symbols. ( Symbols which machine takes as input )
- q : Initial state. ( Starting state of a machine )
- F : set of final state.
- δ : Transition Function, defined as δ : Q X Σ --> Q.

In a DFA, for a particular input character, the machine goes to one state only. A transition function is defined on every state for every input symbol. Also in DFA null (or ε) move is not allowed, i.e., DFA cannot change state without any input character. 

# 2. Nondeterministic Finite Automata(NFA):

NFA is similar to DFA except following additional features: 
- Null (or ε) move is allowed i.e., it can move forward without reading symbols. 
- Ability to transmit to any number of states for a particular input. 

However, these above features don’t add any power to NFA. If we compare both in terms of power, both are equivalent. 

Due to the above additional features, NFA has a different transition function, the rest is the same as DFA.

- δ: Transition Function
- δ:  Q X (Σ U ε ) --> 2^Q.

As you can see in the transition function is for any input including null (or ε), NFA can go to any state number of states.

Since all the tuples in DFA and NFA are the same except for one of the tuples, which is Transition Function (δ)

In case of DFA
- δ : Q X Σ --> Q
In case of NFA
- δ : Q X Σ --> 2^Q
