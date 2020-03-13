InterView Answers

Explain in detail the workings of a dynamic array:
* What is the runtime complexity to access an array, add or remove from the front, and add or remove from the back?
* What is the worse case scenario if you try to extend the storage size of a dynamic array?


* A dynamic array is a contiguious block of memory with elements that are all the same type. 
* Each item can be accessed by the function itemAddress = arrayStartAddress + (itemIndexLocation * sizeOfType)
* Access time is O(1)
* Delete or add to the head is O(n)
* Delete or add to the tail is O(1)
* If the dynamic array is not managed, the worst case for adding an item is if the array is full, in that case the array
will have to be resized which will cost O(n) time.

Explain how a blockchain is structured. What are the blocks, what is the chain? How is the data organized?
 
* The Blockchain is structured where each block contains information that is fixed in time, and cannot be disputed.
* A major use of the blockchain system is that of Financial transactions.
* Each block is similar to the node of a linked list struture, where each block contains information about the previous block.
* Each link in the chain contains a cryptographic hash of the previous block which prevents the previous block from being changed.
* In order to change a block's information then the block has to be reproven, and a cryptographic hash needs to be proven for each successive block that has already been proven.
* The Proof of work is used to validate the block. 
 
Explain how proof of work functions. How does it operate. How does this protect the chain from attack. What kind of attack is possible?

* Individual proofs can only be done by brute force, and are difficult to solve.
* The work is horizontally scaled across several miners that are all searching for a proof.
* This is in order to spread the load and solve the problem in a shorter amount of time.
* This will protect the chain from 1 individual changing the blockchain by changing and remining blocks.
* If one miner gains access to over half of the combined resources, that would give that miner the ability to potentially change the past blocks and take over the blockchain.