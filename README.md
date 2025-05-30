## 📚 Person Record Management using AVL Tree, BST, and B-Tree

This project implements a complete record management system using three different types of tree-based data structures: **AVL Tree**, **Binary Search Tree (BST)**, and **B-Tree**. The goal is to provide a comparative understanding of these data structures in terms of insertion, deletion, searching, and balancing mechanisms, all applied to a real-world use case—managing `Person` records (with ID, Name, and Age).

---

### ⚙️ Features

* 📄 **Person Record Structure**:
  Each record includes:

  * `ID` (int)
  * `Name` (string)
  * `Age` (int)

* 🌳 **AVL Tree**:
  Self-balancing binary search tree with automatic height-based rotations.

* 🌲 **Binary Search Tree (BST)**:
  Standard unbalanced binary tree with recursive insertion, deletion, and search.

* 🌴 **B-Tree**:
  Generalized m-way tree for managing large datasets efficiently. Customizable max degree.

* 🔎 **Operations Supported**:

  * Insert a Person
  * Search by ID
  * Delete by ID
  * In-order Traversal (ascending order by ID)

* 📊 **Performance Comparison** *(optional enhancement)*:
  You can integrate timing and operation counts to compare tree efficiency.

---

### 🧪 Example Usage

```cpp
// Create tree instances
AVLTree avl;
BSTree bst;
BTree btree(3); // B-tree of degree 3 (max 2 keys per node)

// Insert sample data
avl.insert(10, "Alice", 25);
bst.insert(10, "Alice", 25);
btree.insert(10, "Alice", 25);

// Search
avl.search(10);
bst.search(10);
btree.search(10);

// Delete
avl.remove(10);
bst.remove(10);
btree.remove(10);
```

---

### 📁 Project Structure

```
├── avl_tree.cpp
├── bst.cpp
├── btree.cpp
├── main.cpp
├── Makefile
└── README.md
```

---

### 🚀 How to Run

1. **Compile** using the provided Makefile:

```bash
make
```

2. **Run the program**:

```bash
./main
```

3. **Follow the on-screen menu** to insert, delete, search, and display records using different trees.

---

### 🔍 Comparison Criteria (Suggested)

You can compare AVL, BST, and B-Tree on:

* **Balance & Structure**
* **Search Efficiency**
* **Insertion/Deletion Time**
* **Space Usage**
* **Scalability (e.g., for databases, B-Tree excels)**

---

### 📌 Educational Use

This project is ideal for students and educators studying:

* Data Structures and Algorithms
* Tree Traversals and Balancing Techniques
* Database Indexing Concepts (B-Trees)
* Real-world application of Trees in record management
