---
tags:
  - learning
  - programming
created: 2026-05-16
---
# Idea

**What is a Garbage Collector?**:
In computer science a garbage collector is a from *automatic memory management*
This want to recuperate a memory assigned but this is not used for the program. 

>[!note]
>Such the memory not used is called *garbage*
## Concept
This can explain how a automatic memory management, this handle a not longer memory used in the program.

---

## Expanation 
We cam imaginate a memory ram, in this memory we store in memory RAM variables, objects, instances, etc. All this take up a space in memory. 
![[Garbage Collector Example 1.excalidraw]]
And we don't have infinite memory for save all variables or objects in the program. For handle this automatically the modern languages program integrate a Garbage Collector.
![[Garbage Collector Example 2.excalidraw]]

This work analyze the space used for the program and if the variable that no used or not referenced in the program later on, this releases the space of memory
![[Garbage Collector Example 3.excalidraw]]

---
## Relationship 

- [[Rust]]

---

## aplication
The applications of this functionalities is in a lot languages modern how python, java, c# and Scripting languages. This simplifies the work of developers when they make a application. Where they don't have to worry about memory management.

---