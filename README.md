# Day35-50-days-coding-challenge

✅ Problems Covered:

1️⃣ Lowest Common Ancestor of a Binary Tree  
2️⃣ Number of Segments in a String

---

🌳 Problem 1: Lowest Common Ancestor of a Binary Tree

📌 Problem:
Given a binary tree and two nodes p and q, return their lowest common ancestor (LCA).  
The LCA is defined as the lowest node in the tree that has both p and q as descendants.  
A node can be a descendant of itself.

🔍 Approach:
- Traverse the tree using post-order DFS.
- If the current node is p or q, return the current node.
- Recurse on the left and right subtrees.
- If both left and right return non-null, the current node is the LCA.
- If one of them is null, return the non-null result (could be p or q or their LCA).

🧪 Example:
Input: root = [3,5,1,6,2,0,8,null,null,7,4], p = 5, q = 1  
Output: 3

💡 Complexity:
- Time: O(n), where n is the number of nodes in the tree.
- Space: O(h), where h is the height of the tree (due to recursion stack).

---

🔤 Problem 2: Number of Segments in a String

📌 Problem:
Given a string s, return the number of segments in the string.  
A segment is a contiguous sequence of non-space characters.

🔍 Approach:
- Use Python's split() function which automatically handles multiple spaces.
- Count the number of non-empty segments returned.

🧪 Examples:
Input: "Hello, my name is John" → Output: 5  
Input: "Hello" → Output: 1  
Input: "   fly me   to   the moon  " → Output: 5

💡 Complexity:
- Time: O(n), where n is the length of the string.
- Space: O(n), in the worst case, for storing the list of segments.

---

🧠 Key Learnings:
- Recursive thinking is powerful for tree-based problems.
- Built-in functions like split() simplify string manipulation significantly.
- Binary tree traversal can reveal elegant, minimal solutions to complex hierarchical questions.
