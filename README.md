# 🌳 B+ Tree Implementation in C

This project implements a **B+ Tree** data structure in **C**, supporting insertion, search, and level-order display operations.
The implementation is designed for efficient **balanced indexing** with a fixed bucket size, using **node splitting** to maintain balance during insertions.
The project is interactive, allowing users to insert values and display the tree structure level by level.

---

## 📌 Features

* ✅ **Insert Operation** – Adds keys into the B+ Tree while maintaining balance.
* ✅ **Search Operation** – Finds a given key in the tree efficiently.
* ✅ **Level-Order Display** – Prints the tree structure level by level.
* ✅ **Dynamic Memory Management** – Allocates and links nodes dynamically.
* ✅ **Node Splitting** – Handles overflow by splitting leaf and internal nodes.
* ✅ **Interactive Menu** – User-friendly terminal interface.

---

## 🛠️ How It Works

### **Bucket Size**

* The maximum number of keys per node is controlled by the `bucketSize` constant.
* When a node exceeds `bucketSize`, it is **split** into two nodes, and the middle key is pushed up.

### **Main Operations**

1. **Insert**

   * Inserts a key into the appropriate leaf node.
   * Splits nodes when they overflow, propagating changes upward.
2. **Search**

   * Traverses the tree from root to leaf to check if a key exists.
3. **Display**

   * Uses a **queue-based BFS** approach to print the tree level by level.

---


## 📚 Data Structure Overview

* **Node Structure**

  * Stores an array of keys.
  * Stores an array of child pointers.
  * Boolean flag to indicate **leaf** or **internal** node.
* **B+ Tree Properties**

  * All data is stored in **leaf nodes**.
  * Internal nodes store keys for guiding searches.
  * Balanced structure for logarithmic time operations.

---

## 🚀 Future Improvements

* Add **deletion** operation.
* Implement **persistent storage**.
* Enhance display format with better visualization.
