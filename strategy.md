# Leetcode Strategy

### **The Ultimate 7-Step Strategy to Solve DSA Problems**

A robust approach to solving Data Structures and Algorithms (DSA) problems requires careful planning, implementation, and optimization. Here's a **detailed, time-bound guide** with examples to help you excel:

---

### **Step 1: Deep Problem Understanding (5–10 minutes)**

### **What to Do:**

- **Read the Problem Statement:**
Read the problem **2–3 times** to grasp inputs, outputs, and constraints clearly.
- **Highlight Key Points:**
Identify key details like edge cases, constraints, and requirements.
- **Ask Questions:**
    - What is the input?
    - What is the output?
    - Are there specific constraints (e.g., maximum array size, time limits)?
    - Are negative numbers, empty inputs, or duplicate values allowed?

### **Example:**

**Problem:** Find the longest increasing subsequence in an array.

- Input: `[10, 9, 2, 5, 3, 7, 101, 18]`
- Output: Length of the subsequence: `4` (Subsequence: `[2, 3, 7, 101]`)
- Constraints: Array size ≤ 2500, elements ≤ 10^4.

### **Checklist to Write Down:**

1. Input format (e.g., array of integers).
2. Output requirements (e.g., length of subsequence).
3. Edge cases (e.g., empty array, single element).

---

### **Step 2: Devising a Strategy (10–15 minutes)**

### **What to Do:**

- **Identify the Problem Type:**
    - Is it an optimization problem (Dynamic Programming)?
    - Is traversal required (Graph algorithms)?
    - Is sorting helpful (Greedy approach)?
- **Choose the Right Data Structure:**
    - For quick lookups: **HashMap/HashSet**.
    - For sequences: **Dynamic Arrays (e.g., Vectors)**.
    - For hierarchical problems: **Trees** or **Graphs**.
    - For priority-based problems: **Heaps**.
- **Write Down Possible Approaches:**
    - Start with a brute-force approach.
    - Explore optimized algorithms (e.g., divide-and-conquer, binary search).

### **Example:**

For the **longest increasing subsequence**:

1. Brute-force: Generate all subsequences (O(2^N)).
2. Optimized DP: Use `dp[i]` to store the LIS ending at `i` (O(N²)).
3. Optimal Solution: Binary search + DP with a list (O(N log N)).

---

### **Step 3: Breaking Down the Problem (10–15 minutes)**

### **What to Do:**

- Divide the solution into smaller, manageable subtasks.
- List the steps sequentially, ensuring they align with your strategy.
- Write pseudo-code for clarity.

### **What to Write While Breaking Down:**

1. Steps to preprocess the input (e.g., sort the array).
2. Logic for iterative or recursive calls.
3. Handling of edge cases.

### **Example (Pseudo-code for LIS):**

1. Create an empty list `subsequence`.
2. Iterate through the array:
    - If current element > last element of `subsequence`, append it.
    - Else, replace the element in `subsequence` using binary search.
3. Return the length of `subsequence`.

---

### **Step 4: Writing Pseudocode (10–15 minutes)**

### **What to Do:**

- Translate the breakdown into **structured pseudocode**.
- Ensure each line maps directly to a coding construct.
- Write modular code to handle tasks like sorting, searching, etc.

### **Example Pseudocode for LIS:**

```
Initialize subsequence = []
For each num in array:
    If num > last element of subsequence:
        Append num to subsequence
    Else:
        Replace the smallest element in subsequence > num
Return length of subsequence
```

---

### **Step 5: Coding and Debugging (20–30 minutes)**

### **Coding:**

- Stick to the pseudocode and implement it in your chosen language.
- Start with basic functionality and test incrementally.

### **Debugging:**

- **Common Errors:** Index out-of-bound errors, incorrect loop conditions, incorrect edge case handling.
- **Debugging Tips:**
    - Print intermediate outputs to check logic flow.
    - Use IDEs with debugging tools to trace the code line by line.

### **Example Debugging for LIS:**

- Test with: `[10, 9, 2, 5, 3, 7, 101, 18]` → Expected Output: `4`.
- Edge Cases:
    - Empty array → Expected Output: `0`.
    - Single element → Expected Output: `1`.

---

### **Step 6: Iterative Optimization (15–20 minutes)**

### **What to Do:**

- Analyze the current solution's complexity (time and space).
- Identify bottlenecks using profiling tools or test cases.
- Transition to a more efficient approach (e.g., O(N log N) from O(N²)).

### **Optimizing the Example:**

- From O(N²) DP, use Binary Search + DP for O(N log N).
- Replace linear traversal with binary search for placement.

---

### **Step 7: Process Review (5–10 minutes)**

### **What to Do:**

- Reflect on the approach and note learnings.
- Write down similar problems you've solved to build pattern recognition.

### **Example Review Notes:**

- The problem is similar to "Longest Increasing Path in a Matrix".
- Techniques learned: Binary search, use of DP arrays, edge case handling.

---

### **Time Allocation Summary:**

| **Step** | **Time Investment** |
| --- | --- |
| Problem Understanding | 5–10 minutes |
| Devising a Strategy | 10–15 minutes |
| Breaking Down the Problem | 10–15 minutes |
| Writing Pseudocode | 10–15 minutes |
| Coding and Debugging | 20–30 minutes |
| Iterative Optimization | 15–20 minutes |
| Process Review | 5–10 minutes |

---

### **Key Insights for Similar Problems**

1. **Identify Problem Categories:**
    - Subarray problems → Use sliding window or prefix sums.
    - Graph traversal → Use BFS/DFS.
    - Optimization → Use DP or greedy algorithms.
2. **Explore Edge Cases:**
    - Test for corner cases and constraints, e.g., array size of 1, negative numbers.
3. **Develop Pattern Recognition:**
    - Solve 3–5 problems of a similar type to build intuition.
    - Example: Solve "LIS", "Longest Common Subsequence", and "Longest Palindromic Subsequence".

By following this structured, time-managed approach, you can tackle any DSA problem efficiently and build long-term expertise. 🚀
