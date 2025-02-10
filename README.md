# Audting Solidity Contracts
Smart contracts tutorials and info for learning essential auditing skills. 


Roadmap to Audit Solidity Smart Contracts
=========================================

NB: This roadmap is largely based on the roadmap by @0kage_eth. Massive thanks for the roadmap! You can find it here: https://twitter.com/0kage_eth/status/1640795987152375808 (I believe by typing/writing it down will help in understanding/retaining core knowledge)

Estimated time to build necessary skills is around 12-26weeks depending on your experience levels in each of the topics and time available.

1. Understand EVM 
2. Learn Solidity Concepts
3. Learn Foundry
4. Interact with Web3 protocols
5. Master writing test cases
6. Understand Security issues and read reports
7. Practice CTF's


  Learning Solidity
  =================

  These videos are a great intro to blockchain and solidity by Patrick Collins. Don't rush and pace yourself over a few days or weeks and build up your 
  knowledge and experience. 
  
  1. Learn Solidity, Blockchain Development, & Smart Contracts | Powered By AI - Full Course (0 - 6) - https://www.youtube.com/watch?v=umepbfKp5rI
  2. Learn Solidity, Blockchain Development, & Smart Contracts | Powered By AI - Full Course (7 - 11) - https://www.youtube.com/watch?v=sas02qSFZ74
  3. Learn to Code Blockchain DApps by Building Simple Games - https://cryptozombies.io/
  4. Roadmap for Web3/Smart Contract Hacking | 2022 - https://sm4rty.medium.com/roadmap-for-web3-smart-contract-hacking-2022-229e4e1565f9

  IDE's
  =====
   1. Remix (great intro to smart contracts & testing) https://remix.ethereum.org
   2. WebStorm (If you are a student, all the IDE's are free for non-commerical use)
   3. Visual Code
    
  Unit Testing/Deployment/Management Frameworks (Functional)
  ==================
   1. Truffle - Truffle, The most comprehensive suite of tools for smart contract development
      1.1 https://archive.trufflesuite.com/
   3. Hardhat
   4. Foundry - Foundry is a smart contract development toolchain.
      1.1 https://book.getfoundry.sh/
   6. OpenZepplin
    
  Security Based Testing
  ======================
   Static Testing Tools
    
   Static testing is the process of testing smart contracts via code inspection, looking for weaknesses in code potentially leading to exploits.
     1. rand tool
    
   Dynamic Testing Tools
    
   Dynamic testing is the process of testing smart contracts on (ideally) test networks by fuzzing contracts, passing out of bounds arguments etc. 
     1. rand tool 1
      
 
  Well known Vulns
  ================  
  
  1. Reentrancy Attacks
     This occurs when a contract calls an external function that can re-enter the original contract before the initial call is completed.
     Use a checks-effects-interactions pattern, where state changes occur before external calls.
     https://medium.com/coinmonks/reentrancy-exploit-ac5417086750

  2. Integer Overflow and Underflow
     These occur when arithmetic operations result in values exceeding the maximum or minimum representable by the data type.
     Use the SafeMath library or Solidity 0.8+, which has built-in overflow and underflow checks.
     https://faizannehal.medium.com/how-solidity-0-8-protect-against-integer-underflow-overflow-and-how-they-can-still-happen-7be22c4ab92f

  3. Denial of Service (DoS) Attacks
     These attacks aim to make a contract unavailable by consuming excessive resources or triggering infinite loops.
     Avoid complex loops and recursive calls, and set appropriate gas limits.
     https://docs.soliditylang.org/en/v0.8.21/

  4. Front-running Attacks
     Attackers observe pending transactions and submit their own transactions with higher gas fees to be executed before the original.
     Use techniques like time-based locks or randomness to make it difficult for attackers to predict transaction order.
     https://docs.soliditylang.org/

  5. Access Control Vulnerabilities
     These occur when unauthorized parties can access or modify contract data.
     Implement proper access control mechanisms, such as ownership checks and role-based access control.
     https://docs.soliditylang.org/

  6. Timestamp Dependence
     Relying on timestamps can be risky due to potential manipulation or inaccuracies.
     Use block numbers or other deterministic values instead of timestamps.
     https://consensys.github.io/smart-contract-best-practices/development-recommendations/solidity-specific/timestamp-dependence/

  7. Unchecked External Calls
     Failing to check the return value of external calls can lead to vulnerabilities.
     Always check the return value of external calls and handle failures appropriately.
     https://sm4rty.medium.com/unchecked-call-return-value-solidity-security-1-fe794a7cdb6f

  8. Integer Divison by Zero
     Dividing by zero can cause unexpected behavior or errors.
     Check for division by zero before performing the operation.
     https://docs.soliditylang.org/

  9. Gas Limit Manipulation
     Attackers can exploit vulnerabilities in gas limit calculations to drain funds or execute malicious code.
     Set appropriate gas limits and carefully consider gas costs during development.
     https://medium.com/valixconsulting/solidity-security-by-example-10-denial-of-service-with-gas-limit-346e87e2ef78

  10. Reentrancy Attacks (Repeated)
      This is a common vulnerability where a contract can be re-entered during a transaction, leading to unexpected behavior.
      Use a checks-effects-interactions pattern or a reentrancy guard to prevent this.
      https://medium.com/coinmonks/reentrancy-exploit-ac5417086750

    
  Securing Contracts
  ==================
   1. Bug bounties
   2. Formal verification of contracts - https://runtimeverification.com/blog/how-formal-verification-of-smart-contracts-works/

  Bug Bounty Progammes
  ====================

  1. Immunefi Bug Bounty Platform - https://immunefi.com/
  2. Expert web3 bug bounty and crowdsourced audit platform  - https://hackenproof.com/
  3. Ethereum Bug Bounties - https://ethereum.org/en/bug-bounty/ 
   
  Other Great Resouces
  ====================
   1.  Jean Cvllr (smart contract enginner) - https://github.com/CJ42
   2.  Ethereum smart contract testing guide - https://ethereum.org/en/developers/docs/smart-contracts/testing/
   3.  TovarishFin's Smart Contract Boilerplate - https://github.com/TovarishFin/smart-contract-boilerplate
   4.  A must read plan by @0kage_eth for learning auditing skills - https://twitter.com/0kage_eth/status/1640795987152375808
   5.  Blockchain, Solidity tutorial (32hrs of content, focus on your specific needs) - https://www.youtube.com/watch?v=gyMwXuJrbJQ
   6.  Merkle Trees in Blockchain (2mins and worth a watch!) - https://www.youtube.com/watch?v=fB41w3JcR7U
    

  Books
  =====
  
  Before splashing out on expensive books, I normally buy older edtions of books for core information and as I progress purchase new books in specific areas. 
  
  1.  Mastering Blockchain - Second Edition: Distributed ledger technology, decentralisation and smart contracts explained. You should be able to pick up a s/h copy from ebay for $7-8



