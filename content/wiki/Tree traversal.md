---
tags: data.structures algorithms trees
---

While [depth-first search](/wiki/depth-first_search) ([DFS](/wiki/DFS)) and [breadth-first search](/wiki/breadth-first_search) ([BFS](/wiki/BFS)) refer to means of finding nodes within a tree (or graph), [traversal](/wiki/traversal) refers to the exhaustive exploration of a tree (or graph); ie. every node is visited in a traversal.

Traversal may employ [DFS](/wiki/DFS) or [BFS](/wiki/BFS), but [DFS](/wiki/DFS) and [BFS](/wiki/BFS) do not necessarily imply full traversal.

For [depth-first search](/wiki/depth-first_search) there are three main orderings of traversal:

# Pre-order

Children are visited before their parent node:

    (3rd)   B
           / \
    (1st) A   C (2nd)

Pseudo-code:

    def visit(node)
      visit(node.left_child)
      visit(node.right_child)
      node.visit
    end

# In-order

Children and their parent are visited in the order they appear in the tree (ie. reading left-to-right):

    (2nd)   B
           / \
    (1st) A   C (3rd)

Pseudo-code:

    def visit(node)
      visit(node.left_child)
      node.visit
      visit(node.right_child)
    end

# Post-order

Children are visited after their parent node:

    (1st)   B
           / \
    (2nd) A   C (3rd)

Pseudo-code:

    def visit(node)
      node.visit
      visit(node.left_child)
      visit(node.right_child)
    end