========== Question ==========  

### Set Matrix Zeroes

<details><summary><b>📄 Description</b></summary><br>

Given an `m x n` matrix of integers `matrix`, if an element is `0`, set its entire row and column to `0`'s.

You must update the matrix _in-place_.

**Follow up:** Could you solve it using `O(1)` space?

**Example 1:**

![](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/49ffd14e-b32b-4ed8-e0d0-9378e5eb9b00/public)

```
Input: matrix = [
  [0,1],
  [1,0]
]

Output: [
  [0,0],
  [0,0]
]
```

**Example 2:**

![](https://imagedelivery.net/CLfkmk9Wzy8_9HRyug4EVA/04d99cc8-e453-464d-888c-58d0a95daf00/public)

```
Input: matrix = [
  [1,2,3],
  [4,0,5],
  [6,7,8]
]

Output: [
  [1,0,3],
  [0,0,0],
  [6,0,8]
]
```

**Constraints:**

-   `1 <= matrix.length, matrix[0].length <= 100`

-   `-2^31 <= matrix[i][j] <= (2^31) - 1`

</details>

---

Which of these steps is NOT part of the O(1) space solution?

A) Check if the first row and column need to be zeroed

B) Use the first row and column as markers for other cells

C) Create temporary arrays to store which rows and columns contain zeros

D) Process the matrix except the first row and column, then handle those separately  

========== Answer ==========  

**Answer**: C

Creating temporary arrays would require O(m+n) extra space, which violates the O(1) space constraint. The O(1) solution instead uses the first row and column of the matrix itself as markers, avoiding any additional data structures.

========== Id ==========  
251

---

DECK INFO

TARGET DECK: Data Structures and Algorithms::Leetcode::MNAB - Neetcode 150 and blind 75 - multi-author::Part XVIII - Math Geometry::Chapter 3 - Set Matrix Zeroes - Blind

FILE TAGS: #DSA::#Leetcode::#MNAB-Neetcode-150-and-blind-75-multi-author::#Part-XVIII-Math-Geometry::#Chapter-3-Set-Matrix-Zeroes-Blind::#251-Set-matrix-zeroes-details-summary-b

Tags:

Reference:

Related:

```dataview
LIST
where file.name = this.file.name
```

QUESTION STATUS: Safe to store
