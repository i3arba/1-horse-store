# Cyfrin - Assembly & Formal Verification Course

## Horse Store

### Session Goal
1. Write a basic simpleStorage/horse store

### Disclaimer
Please be aware that this readme is basically a notepad. If you want to read my notes, keep going. If not, you can go directly to the code.

#### Questions

1. Where did this data come from? How did Remix know to send this data?
- In the foundry full course we learned that if we take the function name + param, we can transform it into the machine readable function signature
    `cast sig "updateHorseNumber(uint256)`. When we call the function, solidity does a Function Dispatch/Method Dispatch to execute the function and send the data.

    - **What is Function Dispatch/Method Dispatch?**
        - The algorithm used to determine which functions/commands should be run/invoked in response to a message.
        - In the EVM, this is when a smart contract uses the first 4 bytes of a calldata to determine which function(which is a group of opcodes) to send the calldata to.
    - **How does the EVM know how to interpret/interact with data?**

2. How does Remix know to update this number of horses with this data?