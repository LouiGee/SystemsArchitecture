# Systems Architecture

## Exam Structure 
25% Coursework (4 Practicals) and 75% Examination

## Term Coursework Structure 

##### Advanced Java A1 - 01/11/2024 
##### Networks Computer-based test (app. 1 hour) (20%) Deadline - 01/11/2024
##### System Architecture Quiz 1 - Deadline 01/11/2024
##### Machine Learning Assessment 1 - Deadline 18/11/2024
##### Advanced Java A2 - 25/11/2024
##### System Architecture Quiz 2 - Deadline 29/11/2024
##### System Architecture UNIX Assessment - Deadline 09/12/2024
##### System ArchitectureQuiz 3 - Deadline 13/12/2024
##### Networks Problem solving exercises (30%) Deadline - 13/12/2024
##### Machine Learning Assessment 2 - Deadline 13/01/2024


## Target hours revision 
**Target**: 150 \
**Current**: 17\
**Hours per day needed**: ?

### Glossary 

##### RISC architecture 
Reduced Instruction Set Computer. Utilises a small, optimised set of instructions rather than a more complex specialised set. Example - ARM 
##### CISC architecture 
Complex Instruction Set Computer. Aims to minimise number of instructions per program. Complex Instructions, Variable length instructions, Rich adressing modes, microprogramming. Example - x86.
##### ALU 
Arithmetic logic unit. Located in CPU. Arithmetic, logical, bitwise and comparison operations complted here.
##### PC/ IP 
Program counter/ Instruction pointer. Located in CPU. Keeps track of memeory adress of the next program to be executed.
##### MMU 
handles virtual memory and caching operations. Address translation (translateslates virtual memory into physical memeory). Enforces access control policies to memory so programs can only access memory asigned to them.
##### Register 
Inside CPU. Small memory( few bytes/kilobytes), fast. Example - used by ALU to fetch operands(+,=,- etc) 
##### Cache 
Between the CPU and RAM. bigger memeory( kB/mB's), slow than register but faster than RAM. Example - Frequently used instructions/ data)
##### RAM  
Located on motherboard near the CPU. instructions transfered via memory bus. Larger memory than caches and registers but slower. But faster than SSD/HD storage.
##### Pages (Virtual memory)
Pages are fixed-size memory blocks used to organise data.
##### Bytes in a page 
4 KB (4096 bytes): This is a standard page size used in many systems.
##### Page Offset  
The page offset is the part of a virtual or physical address that specifies the exact location within a page. The page offset is crucial for efficient memory management, allowing the system to quickly locate specific data within a page
##### Page Frames (Physical memory)
Page frames are fixed-size blocks of physical memory in a computer system. They are a fundamental concept in the implementation of virtual memory.
##### Page Table
A page table is a data structure used in virtual memory systems to map virtual addresses to physical addresses. It plays a crucial role in translating the virtual addresses used by a program into the physical addresses used by the computer’s hardware.
##### Physcial memory
Physical memory (RAM) is divided into small, fixed-size blocks called page frames.
##### Virtual memory 
Each process is given its own virtual address space, which is divided into pages.
The virtual address space is much larger than the physical memory (RAM).
##### Numerically 
To solve something numerically means through approximation/ iteration
##### Heap
The heap is used for allocating memory at runtime, as opposed to compile-time. Unlike the stack, which has a Last-In-First-Out (LIFO) structure, the heap allows for more flexible memory allocation patterns
##### Kernal Space 
Kernel space is a reserved area of memory where the core of the operating system (the kernel) executes and provides its essential services.
##### Stack
A stack is a data structure that follows the Last-In-First-Out (LIFO) principle. This means that the last element added to the stack is the first one to be removed. Used for function call management, including local variables and return addresses.
##### Mmap segment
The mmap segment in a process’s virtual memory is used for memory-mapped files and shared memory. This segment allows files or devices to be mapped directly into the process’s address space, enabling efficient file I/O and inter-process communication
##### BSS segemnt 
The BSS (Block Started by Symbol) segment is a portion of a program’s memory that contains uninitialized global and static variables.
##### Data segment 
Contains initialized global and static variables. These variables have explicit initial values set in the source code.
##### Text Segment
Contains the executable code of the program##### Address Space Layout Randomization (ASLR)



### Practice Test 10/10/2024

![Screenshot 2024-10-13 at 15 55 45](https://github.com/user-attachments/assets/533372dc-0774-4043-bbce-261325b9bdb6)

![Screenshot 2024-10-13 at 15 27 14](https://github.com/user-attachments/assets/94f36c1a-bb85-4ec4-8f64-643e6518d9bd)

![Screenshot 2024-10-13 at 15 28 13](https://github.com/user-attachments/assets/930b2d7a-106e-4ac7-bdc3-b47756961239)


##### Key Characteristics of RISC:
Simplified Instructions: Each instruction is designed to execute in a single clock cycle, which simplifies the processor design and can lead to higher performance.
Load/Store Architecture: Data processing operations are performed only on registers, with separate instructions for loading data from memory into registers and storing data back to memory.
Fixed Instruction Length: Instructions are typically of a uniform length, which simplifies instruction decoding and pipelining.
Large Number of Registers: RISC architectures often have a large number of general-purpose registers to reduce the frequency of memory access.

##### Key Characteristics of CISC:
Complex Instructions: CISC processors have a large number of instructions, some of which can perform multi-step operations or complex tasks within a single instruction.
Variable Instruction Length: Instructions can vary in length, which can make decoding more complex but allows for more flexible and powerful instructions.
Fewer Registers: Compared to RISC architectures, CISC processors typically have fewer general-purpose registers.
Microcode: Many CISC instructions are implemented using microcode, which translates complex instructions into simpler, lower-level operations within the CPU.

![Screenshot 2024-10-13 at 15 28 59](https://github.com/user-attachments/assets/78ded9ab-1fff-4742-a4fd-6df0364c0c4e)

![Screenshot 2024-10-13 at 15 29 08](https://github.com/user-attachments/assets/bd568555-bfb2-4481-90be-6e78cf1c2b0d)


##### Arithmetic Logic Unit (ALU) is a critical component of the CPU responsible for performing arithmetic and logical operations. Here are its main functions:

Arithmetic Operations
Addition: Adding two numbers.
Subtraction: Subtracting one number from another.
Multiplication: Multiplying two numbers.
Division: Dividing one number by another.
Logical Operations
AND: Performing a logical AND operation.
OR: Performing a logical OR operation.
NOT: Performing a logical NOT operation.
XOR: Performing a logical XOR operation.
Bitwise Operations
Shift Left: Shifting bits to the left.
Shift Right: Shifting bits to the right.
Rotate: Rotating bits left or right.
Comparison Operations
Equal To: Checking if two values are equal.
Less Than: Checking if one value is less than another.
Greater Than: Checking if one value is greater than another.
Role in CPU
Data Processing: The ALU processes data from the registers and memory, performing the necessary calculations and logical operations.
Instruction Execution: It executes the instructions provided by the control unit, which directs the ALU on which operations to perform.

![Screenshot 2024-10-13 at 15 30 18](https://github.com/user-attachments/assets/2e4aa941-aa2b-4761-8c9d-979eba4cb206) 1

![Screenshot 2024-10-13 at 15 30 45](https://github.com/user-attachments/assets/fa49700f-c6a2-4446-964b-d15cc1b6d907) 2

![Screenshot 2024-10-13 at 15 31 12](https://github.com/user-attachments/assets/7181a251-d351-4cb0-80c9-e7900d4afee3) 3 

![Screenshot 2024-10-13 at 15 31 35](https://github.com/user-attachments/assets/0875ca72-ff6b-4af0-8c64-692510010bf3) 4 


![Screenshot 2024-10-11 at 16 19 39](https://github.com/user-attachments/assets/3717c95e-9049-45e1-aab0-6bfef8772adf) 5 

![Screenshot 2024-10-13 at 15 34 31](https://github.com/user-attachments/assets/d03c704e-a448-4031-9669-c50ed305355a) 6

![Screenshot 2024-10-13 at 15 34 46](https://github.com/user-attachments/assets/c920c1fd-77bf-4544-860d-83ddf66ec7ad) 7

![Screenshot 2024-10-13 at 15 35 13](https://github.com/user-attachments/assets/31a25966-0c3c-45c5-9825-d60b7aecbaf7) 8 


![Screenshot 2024-10-13 at 15 35 40](https://github.com/user-attachments/assets/913bfb42-7114-4d43-9d27-51049cbd014a) 9 


![Screenshot 2024-10-13 at 15 36 13](https://github.com/user-attachments/assets/a909a307-f862-48f8-8bb3-ba09500218f1) 10 


![Screenshot 2024-10-13 at 15 36 39](https://github.com/user-attachments/assets/45fc18dc-6142-4f52-8be7-5322fa86f400) 11
![Screenshot 2024-10-11 at 16 30 32](https://github.com/user-attachments/assets/db53d1d6-b3df-43f6-86f9-0a744be5ee4a) 12


![Screenshot 2024-10-13 at 15 37 00](https://github.com/user-attachments/assets/d26724f7-95bf-4d0c-a736-54ba9f9f50b8) 13


![Screenshot 2024-10-13 at 15 45 44](https://github.com/user-attachments/assets/be13c4cc-c430-463a-af2a-a06a833acceb) 15

![Screenshot 2024-10-13 at 15 58 01](https://github.com/user-attachments/assets/9969a4c2-412e-4dae-b8a4-ea63dd551bfc)


![Screenshot 2024-10-13 at 16 02 03](https://github.com/user-attachments/assets/60bcb584-e3e4-4729-b817-e5b06638caf2)


![Screenshot 2024-10-11 at 16 34 57](https://github.com/user-attachments/assets/7fb7c476-e2c1-4e8f-9267-36f556ccf169) 18 

![Screenshot 2024-10-11 at 19 27 00](https://github.com/user-attachments/assets/823bfaee-f3a3-4a9f-99c3-2bfd5458a09b) 19

![Screenshot 2024-10-11 at 19 37 44](https://github.com/user-attachments/assets/e85e71f3-e6b5-4d14-8b70-3cd92b14d2f9) 20 

![Screenshot 2024-10-11 at 19 56 26](https://github.com/user-attachments/assets/0a6ad96a-a250-43e5-a5ee-2328e5f08456) 21

![Screenshot 2024-10-13 at 15 49 39](https://github.com/user-attachments/assets/7d6e7a79-abc4-48e7-8358-077ab0988f9f) 22

![Screenshot 2024-10-11 at 20 11 28](https://github.com/user-attachments/assets/6c12a4ce-96c4-40db-9e69-8ca99325e2d7) 23 

![Screenshot 2024-10-13 at 16 04 41](https://github.com/user-attachments/assets/0fb93df2-59d1-4984-938f-5ddbeb05b0b0)


![Screenshot 2024-10-13 at 12 32 48](https://github.com/user-attachments/assets/9452f33a-f0b0-43ff-ad1c-6329fce3c75f) 25

The offset inside a page refers to the specific location within a page where a particular piece of data can be found. In a virtual memory system, both virtual and physical addresses are divided into two parts: the page number and the offset.

A virtual address in a computer is an address used by a program to access memory. It is part of a virtual memory system that allows an operating system to use hardware and software to manage memory more efficiently. Here’s a breakdown of how it works:

Physical Memory:
Physical memory (RAM) is divided into small, fixed-size blocks called page frames.

Virtual Memory:
Virtual memory is divided into pages, which are also fixed-size blocks.

A page table is a data structure used in virtual memory systems to map virtual addresses to physical addresses. 
It plays a crucial role in translating the virtual addresses used by a program into the physical addresses used by the computer’s hardware.

General Formula:
For a page size of ( 2^b ) bytes, the number of bits required for the offset is ( b ).


Key Concepts:
Virtual Memory:
Virtual memory allows a computer to compensate for physical memory shortages by temporarily transferring data from random access memory (RAM) to disk storage.
It creates an illusion for users of a very large (main) memory.
Virtual Address Space:
Each process has its own virtual address space, which is a range of addresses that the process can use.
This space is divided into pages, which are fixed-size blocks of memory.
Translation to Physical Addresses:
The virtual address is translated to a physical address by the Memory Management Unit (MMU).
This translation is done using a page table, which maps virtual addresses to physical addresses.
Benefits of Virtual Addresses:
Isolation:
Each process operates in its own virtual address space, which prevents processes from interfering with each other’s memory.
Security:
Virtual memory provides a layer of security by isolating the memory of different processes.
Efficient Memory Use:
It allows the system to use physical memory more efficiently by swapping inactive pages to disk and keeping active pages in RAM.

Solving numerically means finding an approximate solution to a mathematical problem using numerical methods rather than exact algebraic expressions. This approach is often used when an equation is too complex to solve analytically or does not have a closed-form solution. Here are some key points about numerical solutions:

Key Concepts:
Approximation:
Numerical methods provide approximate solutions that are often very close to the exact solution.
The accuracy of the solution depends on the method used and the computational resources available.
Iterative Methods:
Many numerical methods are iterative, meaning they start with an initial guess and refine it through repeated calculations.
Examples include the Newton-Raphson method, bisection method, and fixed-point iteration.
Computational Tools:
Numerical solutions are typically found using computers and specialized software or programming languages like Python, MATLAB, or R.
These tools can handle complex calculations and large datasets efficiently.

![Screenshot 2024-10-13 at 13 24 07](https://github.com/user-attachments/assets/1dd22b76-cc55-409d-bfe0-1ee19da400de)

![Screenshot 2024-10-13 at 13 26 21](https://github.com/user-attachments/assets/981e78b4-2c8f-49bd-b534-062d26ee89f1)

This statement is true due to the Pigeonhole Principle. Here’s why:

Suppose there are ( n ) objects in the heap.
Each object points to at least one other object, so the number of objects each object can point to ranges from 1 to ( n-1 ).
This gives us ( n ) objects and ( n-1 ) possible values for the number of objects each object can point to. According to the Pigeonhole Principle, if you have more objects (pigeons) than possible values (pigeonholes), at least two objects must point to the same number of other objects.

Therefore, in this heap, there must be at least two objects that point to the same number of other objects.


![Screenshot 2024-10-13 at 13 28 54](https://github.com/user-attachments/assets/4971ad5c-6ec3-4b2f-9c4d-d0ccdd2e2c22)

While using multiple threads can improve the performance and responsiveness of a program, it doesn’t necessarily increase its reliability. In fact, multithreading can introduce complexity and potential issues such as race conditions, deadlocks, and synchronization problems.

![Screenshot 2024-10-13 at 13 30 31](https://github.com/user-attachments/assets/effae050-ea21-4f90-ba40-27c919698f22)

![Screenshot 2024-10-13 at 13 31 58](https://github.com/user-attachments/assets/8b888627-321a-4280-840e-43101973be25)

![Screenshot 2024-10-13 at 13 32 38](https://github.com/user-attachments/assets/4dba1737-781b-43b4-ab4b-cbcb68a9562e)

![Screenshot 2024-10-13 at 13 40 20](https://github.com/user-attachments/assets/7b9da765-02fb-4c24-a145-a842e97e2e89)

Yes, that’s correct! The virtual memory of a process is organized into several segments, each serving a specific purpose. Here’s a brief overview of each segment and the concept of address space randomization:

Segments in Virtual Memory:
Kernel Space:
Reserved for the operating system kernel and its data structures.
Not accessible by user processes.
Stack:
Used for function call management, including local variables, return addresses, and control flow.
Grows downward in memory.
The starting position is usually randomized for security reasons (stack randomization).
Mmap Segment:
Used for memory-mapped files and shared memory.
Allows files or devices to be mapped into the process’s address space.
The starting position is usually randomized (mmap randomization).
Heap:
Used for dynamic memory allocation (e.g., via malloc in C).
Grows upward in memory.
The starting position is usually randomized (heap randomization).
BSS Segment:
Stands for “Block Started by Symbol.”
Contains uninitialized global and static variables.
Initialized to zero by the operating system.
Data Segment:
Contains initialized global and static variables.
Values are set at compile time.
Text Segment:
Contains the executable code of the program.
Typically read-only to prevent accidental modification.
Address Space Layout Randomization (ASLR):
ASLR is a security technique used to randomize the starting addresses of key memory segments (stack, mmap, heap) each time a program is executed.
This makes it more difficult for attackers to predict the location of specific functions or data structures, thereby enhancing security against certain types of attacks, such as buffer overflows.

![Screenshot 2024-10-13 at 13 42 21](https://github.com/user-attachments/assets/9b1faac7-7eb9-4a1e-9988-456e28528518)

![Screenshot 2024-10-13 at 13 50 52](https://github.com/user-attachments/assets/30f49c2a-9f7a-45cf-a4e9-54eb32e2ec52)

![Screenshot 2024-10-13 at 13 50 17](https://github.com/user-attachments/assets/725564b9-76fc-4e6b-8fe4-76e02f021937)

![Screenshot 2024-10-13 at 13 58 22](https://github.com/user-attachments/assets/1222cc7c-4819-4599-9826-e6ff0d6b058e)

If we compile an integer addition ( x + y ) into an add instruction followed by a decrement, we will always get the correct answer in OCaml. The decrement operation adjusts the result to match the OCaml integer representation, ensuring that the LSB is set to 1

![Screenshot 2024-10-13 at 15 53 30](https://github.com/user-attachments/assets/a9a01918-4e46-4172-92cc-0ab7466f85db)

![Screenshot 2024-10-13 at 14 15 50](https://github.com/user-attachments/assets/92fa4225-fcf8-41ea-829d-de0d24658ead)

![Screenshot 2024-10-13 at 14 21 38](https://github.com/user-attachments/assets/702a5e75-eb37-4270-aa1e-8d2f33c5e399)

![Screenshot 2024-10-13 at 14 22 09](https://github.com/user-attachments/assets/0391b85a-c905-4bb6-9310-1067f557b11d)

![Screenshot 2024-10-13 at 14 24 16](https://github.com/user-attachments/assets/59818cb1-6ffd-4088-8179-ad9f5095f33b)


### Lecture 1 & 2 - introduction; numbers and logic 25/09/2024
![Screenshot 2024-10-07 at 09 51 00](https://github.com/user-attachments/assets/c5790a7f-487e-4d52-ad39-1bfb4513cb40)

![Screenshot 2024-10-07 at 09 48 01](https://github.com/user-attachments/assets/21f9fa36-969d-4bb7-9093-c3fcbfbbfacd)

![Screenshot 2024-10-07 at 09 49 09](https://github.com/user-attachments/assets/33fe2ea2-bc03-4839-8636-a362ac50173a)

![Screenshot 2024-10-07 at 09 54 48](https://github.com/user-attachments/assets/f76e5027-a9a6-4067-b626-eb5f4c409d02)

![Screenshot 2024-10-07 at 09 56 33](https://github.com/user-attachments/assets/3c5ca21e-82c4-48b7-91c7-ad5f49321eec)

![Screenshot 2024-10-07 at 09 57 03](https://github.com/user-attachments/assets/c09d5087-8802-4d02-8de3-a024cefa2cc1)

![Screenshot 2024-10-07 at 09 58 08](https://github.com/user-attachments/assets/011517ed-f8ac-441f-b53b-1f66fd73109f)

![Screenshot 2024-10-07 at 09 58 55](https://github.com/user-attachments/assets/ee5e3469-5cf8-4b15-ac82-6373862b91b5)

![Screenshot 2024-10-07 at 10 00 36](https://github.com/user-attachments/assets/9eb343a7-9722-4c99-babe-b4e96e323b67)

![Screenshot 2024-10-07 at 10 00 56](https://github.com/user-attachments/assets/64a18d5a-d247-410c-acb2-340daae76cd9)

![Screenshot 2024-10-07 at 10 02 23](https://github.com/user-attachments/assets/14a8cd11-09c1-43cc-af69-42c3aed7af95)

![Screenshot 2024-10-07 at 10 02 49](https://github.com/user-attachments/assets/65cd4503-fe10-4346-acc8-43c417678924)

Superposition - idea that allows for qubits to exist in multiple states, particles can be in multiple states at once.

Quantum entanglement - Where two or more particles become interconnected in such a way that the state of one particle instantly influences the state of the other, no matter how far apart they are.

![Screenshot 2024-10-07 at 10 20 00](https://github.com/user-attachments/assets/a4cef444-b4e7-4d1f-8672-a2b0f75fcee2)

![Screenshot 2024-10-07 at 10 20 20](https://github.com/user-attachments/assets/755796f6-4c64-46c1-8103-8bf7442725d9)

![Screenshot 2024-10-07 at 10 20 50](https://github.com/user-attachments/assets/794c2d55-bd41-4eb6-a10a-908f8ee9604e)

![Screenshot 2024-10-07 at 10 21 50](https://github.com/user-attachments/assets/f2655fd5-1737-4e90-a275-ee2af4e58581)

![Screenshot 2024-10-07 at 10 22 08](https://github.com/user-attachments/assets/4f7d76e8-ae7b-4b4c-aa82-07fb84bbbc90)

![Screenshot 2024-10-07 at 10 22 59](https://github.com/user-attachments/assets/0918f959-4409-406d-bb34-9723adf0cf2d)

![Screenshot 2024-10-07 at 10 23 33](https://github.com/user-attachments/assets/6d029a1c-231f-4fde-a37d-454cc6a6e717)


![Screenshot 2024-10-07 at 09 54 30](https://github.com/user-attachments/assets/0272c153-14dd-43f7-ab0f-bf8dd2a5c01d)

![Screenshot 2024-10-07 at 09 49 44](https://github.com/user-attachments/assets/e761f2dc-e9bd-48a4-8137-517bf4600c7e)

![Screenshot 2024-10-07 at 10 27 52](https://github.com/user-attachments/assets/a79c9b7b-e46f-49ff-81ad-624161fce1fd)


Von Neumann Architecture
Stored-Program Concept: Von Neumann’s architecture is based on the idea that both data and instructions are stored in the same memory. This allows the computer to be reprogrammed without altering its hardware1.
Single Memory Space: Both instructions and data share the same memory and pathways, which simplifies the design but can lead to bottlenecks1.
Sequential Execution: Instructions are fetched, decoded, and executed one at a time, which can limit speed due to the "von Neumann bottleneck"1.
Turing’s Universal Machine
Abstract Model: Turing’s concept of a universal machine is more theoretical. It describes a machine that can simulate any other machine given the correct algorithm and sufficient time2.
Algorithmic Focus: Turing’s work laid the groundwork for understanding algorithms and computation, emphasizing the logical structure of computation rather than physical implementation2.
Flexibility: The Turing machine is a model for what can be computed, providing a foundation for the theory of computation and influencing the development of programming languages2.
Key Differences
Practical vs. Theoretical: Von Neumann’s architecture is a practical design for building computers, while Turing’s machine is a theoretical model that defines the limits of what can be computed21.
Memory Structure: Von Neumann’s architecture uses a single memory for both data and instructions, leading to potential bottlenecks. Turing’s model doesn’t specify memory structure but focuses on the logical steps of computation1.
Impact on Modern Computing: Von Neumann’s architecture directly influenced the design of most modern computers, while Turing’s ideas underpin the theoretical aspects of computer science
<img width="933" alt="Screenshot 2024-09-25 at 15 34 19" src="https://github.com/user-attachments/assets/912fffdc-e93b-413e-95a7-7a44b41b9ba0">

<img width="923" alt="Screenshot 2024-09-25 at 15 35 17" src="https://github.com/user-attachments/assets/39150857-8819-45d7-b105-894d041b82ca">

<img width="800" alt="Screenshot 2024-09-25 at 15 36 47" src="https://github.com/user-attachments/assets/e7705ada-67f3-4a5a-afa2-ea08130ccd02">

<img width="854" alt="Screenshot 2024-09-25 at 15 38 21" src="https://github.com/user-attachments/assets/320761bb-7e79-4689-9d33-da8b239ebd78">

<img width="858" alt="Screenshot 2024-09-25 at 15 41 22" src="https://github.com/user-attachments/assets/a082c1a2-c667-4914-8549-b9e6e74aae07">


### Lecture 3  Gates and arithmetic; boolean algebra; ALU 01/10/2024

<img width="856" alt="Screenshot 2024-09-25 at 15 57 22" src="https://github.com/user-attachments/assets/53047fc9-2423-41c7-a66e-cdd1a36d76e8">

<img width="864" alt="Screenshot 2024-09-25 at 16 03 04" src="https://github.com/user-attachments/assets/5fdb3890-6ecd-44b3-9d1d-ef6ba19c4d43">

![Screenshot 2024-10-07 at 10 34 53](https://github.com/user-attachments/assets/9ea3d62a-fca8-4988-9eaa-1b3e45b8dd03)

![Screenshot 2024-10-07 at 10 35 27](https://github.com/user-attachments/assets/f13294e9-0e42-4b2e-b866-c2050ed2752b)

![Screenshot 2024-10-07 at 10 36 29](https://github.com/user-attachments/assets/ef6de098-a73c-442c-a94c-697860ce9fe5)

![Screenshot 2024-10-07 at 10 36 54](https://github.com/user-attachments/assets/45d9507c-3f0b-4350-bbfe-2afbfd4695fc)

![Screenshot 2024-10-07 at 10 37 12](https://github.com/user-attachments/assets/6f9e51dc-ee6b-4bb7-acc3-9bbefcb09a9b)

![Screenshot 2024-10-07 at 10 37 42](https://github.com/user-attachments/assets/8af9ddca-6d2a-44a2-9ceb-f757dbb70cac)

![Screenshot 2024-10-07 at 10 38 49](https://github.com/user-attachments/assets/c2d61a14-f901-4a36-9363-2f565c9879bf)

![Screenshot 2024-10-07 at 10 39 36](https://github.com/user-attachments/assets/c997b687-d3d9-44de-a8fb-890ecb543c70

![Screenshot 2024-10-07 at 10 42 04](https://github.com/user-attachments/assets/cc4f90f8-8f22-4dbc-9bc9-584c448e6725)

![Screenshot 2024-10-07 at 10 42 50](https://github.com/user-attachments/assets/4db27fa3-f214-4431-bc25-94dc87c5cfbc)

![Screenshot 2024-10-07 at 10 43 26](https://github.com/user-attachments/assets/afe7a967-55b9-4bc0-9f9d-44f177eed3fe)

Inventor of the modern adder Charles babbage

![Screenshot 2024-10-07 at 10 44 21](https://github.com/user-attachments/assets/e23cbf51-aba3-4adb-be2b-0ad7b14ac8c7)

### Lecture 4 & 5  Programs as instructions; numbers; arithmetic; logic & Instruction set architecture 07/10/2024

![Screenshot 2024-10-07 at 11 12 20](https://github.com/user-attachments/assets/1428c3d0-e624-4e6f-84e8-55e49d57d141)

![Screenshot 2024-10-07 at 11 12 35](https://github.com/user-attachments/assets/b425b6fe-4138-44e4-95bb-4a222fb20467)

![Screenshot 2024-10-07 at 11 13 13](https://github.com/user-attachments/assets/59083931-0146-47c7-84d4-615a639cbfea)

![Screenshot 2024-10-07 at 11 17 01](https://github.com/user-attachments/assets/03025a77-b428-4d74-aca8-80024d379888)

![Screenshot 2024-10-07 at 11 18 06](https://github.com/user-attachments/assets/8f4ec633-f74e-46a0-8e5e-a68cdcdec972)

![Screenshot 2024-10-07 at 11 18 14](https://github.com/user-attachments/assets/c929d2db-0a68-4dd8-81cb-68a7db5d4fc0)

0b6 - 0b8

6 = 0110 
Finding the two complement of 8 = 1000 = 0111 = 1000 (add trailing one to 0111)

0110 - 1000 = 1110 (answer given as -2 in twos complement form)


<img width="682" alt="Screenshot 2024-10-07 at 17 02 21" src="https://github.com/user-attachments/assets/6d039963-14fc-45ba-987f-c750572c9f90">

<img width="678" alt="Screenshot 2024-10-07 at 17 02 50" src="https://github.com/user-attachments/assets/7af8f692-ba03-4f91-9af9-113844c2bc3a">

LD is load

<img width="682" alt="Screenshot 2024-10-07 at 17 03 16" src="https://github.com/user-attachments/assets/82d2c873-a9db-420a-886d-a0426816236d">

<img width="673" alt="Screenshot 2024-10-07 at 17 03 41" src="https://github.com/user-attachments/assets/22944a59-11c5-46d9-b933-a533040a32ab">

<img width="452" alt="Screenshot 2024-10-07 at 17 04 38" src="https://github.com/user-attachments/assets/f6a83971-dba3-4631-ac88-466e71629572">

<img width="449" alt="Screenshot 2024-10-07 at 17 05 01" src="https://github.com/user-attachments/assets/8c6d28ac-e81d-4f27-b0e7-cf2ba3f323d1">

LD is load

ALU is arithemetic logic unit

<img width="451" alt="Screenshot 2024-10-07 at 17 05 20" src="https://github.com/user-attachments/assets/3fc935fe-f201-412f-88bf-fa84dc5c4167">

<img width="451" alt="Screenshot 2024-10-07 at 17 05 43" src="https://github.com/user-attachments/assets/482e99fa-f265-47de-881c-3c1e395755ec">

<img width="455" alt="Screenshot 2024-10-07 at 17 06 20" src="https://github.com/user-attachments/assets/751eb872-22a7-4a42-81b7-313b1c7bc26a">

<img width="456" alt="Screenshot 2024-10-07 at 17 06 38" src="https://github.com/user-attachments/assets/a3df5e68-851f-4c06-8881-c509392c81ef">

<img width="455" alt="Screenshot 2024-10-07 at 17 06 59" src="https://github.com/user-attachments/assets/e8f5aa22-0ed2-4d85-b7b3-6335918d4027">

<img width="455" alt="Screenshot 2024-10-07 at 17 07 25" src="https://github.com/user-attachments/assets/3097d313-2aa7-4656-bd1d-416a57bd42ec">

<img width="454" alt="Screenshot 2024-10-07 at 17 07 55" src="https://github.com/user-attachments/assets/3e2e5525-78d8-4e8f-93a0-32fc4ab3a561">

<img width="456" alt="Screenshot 2024-10-07 at 17 08 37" src="https://github.com/user-attachments/assets/c4d76450-d710-4cd5-b065-f23c65fda7e1">

<img width="458" alt="Screenshot 2024-10-07 at 17 09 15" src="https://github.com/user-attachments/assets/8a0bc159-7075-44ca-94db-f802ff458b69">

