#complex_knowledge

Two [[Memory]] layouts, presents  in programming languages.
This concept only make sense in C, C++ and Java?
Well, first of all, there is other areas of memory in those structures (I guess it varies with the language, but some examples are  the Text Segment where the code is stored, and the BSS or uninitialized data segment, where global variables, not initialized and initialized with 0 variables are stored).
So, the stack and the heap are basically the "table" of the memory. The stack is the small, inflexible but easy to access space, like the one right beside the cooking board. The heap is the rest of the table, bigger but harder to grab tings on, and gets really messy if you don't manage it correctly, because thing can be put wherever you want.
One funny thing is that this two spaces grown towards each other, so when they met, the memory is full.
The stack follows the data structure [[stack]], so it's a LIFO space. The heap "has nothing to do with the data structure [[heap]]".
Also, the stack is contiguous, and it's the memory space that allows the recursive function behavior in C (and possibly others).
The heap can grow, occupying more memory if need. The stack, on the other hand, is a fixed size.

It was organized this way because it is kinda easy to implement, and is a good way to work with memory. Maybe there is  more modern and complex methods, but this one still is very good.