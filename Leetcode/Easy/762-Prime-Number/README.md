Problem Overview:
Goal: Find the count of numbers in the inclusive range [left,right] that have a **prime number** of set bits (1s) in their binary representation.
- Key Concept: Bit manipulation and prime number identification.

Approach:
1. Constraints Analysis: 
   - The maximum value of right is 10^6. 
   - Since 2^{20} = 1,048,576, any number in the range will have at most 20 bits as 10^6 = 
2. Pre-defining Primes:
   - Because the maximum number of set bits is only 20, I can pre-define the primes under 20:
   - {2, 3, 5, 7, 11, 13, 17, 19}.
   - This avoids unnecessary complex prime-checking logic (Hard-coding for optimization).
3. Efficient Bit Counting:
   - Used the C++ built-in function __builtin_popcount() which is highly optimized at the compiler level for counting set bits.

Key Takeaways
- Learned that using compiler-specific intrinsics like __builtin_popcount is faster than manual loops because it often maps directly to a single CPU instruction.
- Practiced analyzing data constraints to simplify algorithms, which is a crucial skill for memory-constrained embedded systems.
- STL Usage: Refreshed my knowledge of std::set for efficient checks.

It was a good practice to do after my military service ended. 
