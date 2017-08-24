# Formal Verification of Smart Contracts
Smart contracts are powerful means for enforcing rules which hold, transfer, receive, or spend digital assets. 

Formal verification means applying a proof that the program behaves according to a specification. In general, this is done with a concrete specification language used to describe how input and output of functions should relate.

So why is it important for smart contracts? 
1. smart contracts are immutable, you can't patch them easily, 
2. smart contracts store value and are 
3. accessible publicly from all over the world. 

This makes them very attractive for hacker attacks. Formal Verification is a strong approach to reduce the risk of bugs and attacks.

Formal verification can be quite sophisticated with mathematical models describing the problem, but also very simple. Some consider Unit Testing the simplest form of formal verification. The trick is always to describe the behavior of an algorithm without reproducing it, having an outside look. 

Using formal verification, it is possible to perform an automated mathematical proof that your source code fulfills a certain formal specification. The specification is still formal (just as the source code), but usually much simpler.

Note that formal verification itself can only help you understand the difference between what you did (the specification) and how you did it (the actual implementation). You still need to check whether the specification is what you wanted and that you did not miss any unintended effects of it.

# Ethereum

Ethereum is a framework for cryptocurrencies which uses blockchain technology to provide an open global computing platform, called the Ethereum Virtual Machine (EVM). EVM executes bytecode on a simple stack machine. Programmers do not usually write EVM code; instead, they can program in a JavaScript-like language, called Solidity, that compiles to bytecode. Since the main purpose of EVM is to execute smart contracts that manage and transfer digital assets (called Ether), security is of paramount importance. However, writing secure smart contracts can be extremely difficult: due to the openness of Ethereum, both programs and pseudonymous users can call into the public methods of other programs, leading to potentially dangerous compositions of trusted and untrusted code. This risk was recently illustrated by an attack on TheDAO contract that exploited subtle details of the EVM semantics to transfer roughly $50M worth of Ether into the control of an attacker.

## WhitePapers
* Formal Verification of Smart Contracts by Karthikeyan Bhargavan1, Antoine Delignat-Lavaud2, Cédric Fournet2, Anitha Gollamudi3, Georges Gonthier2, Nadim Kobeissi1, Natalia Kulatova1, Aseem Rastogi2, Thomas Sibut-Pinote1, Nikhil Swamy2, and Santiago Zanella-Béguelin2 http://antoine.delignat-lavaud.fr/doc/plas16.pdf

# Talk
https://www.youtube.com/watch?v=rx0NPckEWGI slides https://chriseth.github.io/notes/talks/formal_ic3_bootcamp/

## Articles
* security page on the solidity documentation https://solidity.readthedocs.io/en/latest/security-considerations.html
* Writing Secure Solidity http://www.blunderingcode.com/writing-secure-solidity/
* Peter Vessenes' blog http://vessenes.com/
* https://github.com/pirapira/ethereum-formal-verification-overview
* https://www.coindesk.com/ethereum-formal-verification-smart-contracts/


## Tools
Formal Verification for Solidity Contracts 

### Oyente
* https://github.com/melonproject/oyente  for bugs detected by the tool http://www.comp.nus.edu.sg/~loiluu/papers/oyente.pdf

### Why 3
* why3. http://why3.lri.fr/

### Securify
* Securify (code, machine code, adress) http://securify.ch/

### Imandra
Imandra analyses algorithms to help you understand what they do, why they do it, and what can possibly go wrong. https://www.imandra.ai/
There is a module to analyse Ethereum EVM code at https://github.com/AestheticIntegration/contracts, watch the blog entry https://blog.benefactory.cc/devcon-2-imandra-contracts-formal-verification-for-ethereum-8e9627bf71f3


### Others
* How to https://gist.github.com/chriseth/c4a53f201cd17fc3dd5f8ddea2aa3ff9
