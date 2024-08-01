# What is Computer Science?

- **Overview of Computer Science**:
    - Comprises many different activities.
    - Divided into three main categories: Theory, Systems, and Applications.
- **Theory**:
    - Theoretical work on what computers can do.
    - Study of what kinds of problems can be computed.
- **Systems**:
    - Study of computers themselves.
    - Building software that runs computers, including operating systems.
    - Design of programming languages.
- **Applications**:
    - Using computers in sophisticated ways to accomplish various tasks.
    - Applications have spread to other fields and are not always labeled as computer science anymore.
- **Thinking Computationally**:
    - Approaching problems by dividing them into tasks that can be performed by a computer.
    - Requires understanding what a computer is and what it can do.
    - Necessitates precise description of tasks since computers do exactly what they are instructed to do.
- **Systems Area**:
    - Building software that runs computers.
    - Examples include the UNIX operating system.
    - Managing data movement from disk drives to RAM and handling program execution.
    - Operating systems manage multiprocessor systems, allowing multiple programs to run simultaneously.
- **Programming Languages**:
    - Tools for communicating with computers.
    - Highly constrained languages with specific defined terms.
    - Popular languages include Python, Perl, C++, and Java.
- **Engineering in Computer Science**:
    - Involves writing good code and testing it.
    - Ensuring the code works under all required conditions and delivers expected results.
    - Preventing program crashes or hangs.
- **Hardware Aspect**:
    - Software must communicate with the actual device.
    - Includes devices like laptops, desktops, mobile phones, and robots.
    - Increasing number of devices are controlled by computer programs.
    - Understanding device behavior benefits from thinking like a computer scientist.

# Algorithms

- **Definition of an Algorithm**:
    - Algorithms describe what a computer can do.
    - Used in computer science and computational biology.
    - An algorithm is a clear, step-by-step series of instructions for completing a task.
    - Algorithms do not necessarily require computers.
- **Example of a Non-Computational Algorithm**:
    - Recipe for making chocolate brownies.
    - Steps: Preheat the oven, melt chocolate chips and butter, cool, stir in eggs and additional ingredients, spread in a pan, bake.
- **Computational Example: Finding a Maximum**:
    - Common in optimization problems.
    - Imagine walking in a landscape to find the highest point.
    - Algorithm: Look for the steepest slope and take a step in that direction.
    - Continue until no further upward steps can be taken.
    - This algorithm finds a local maximum, not necessarily the highest point overall.
- **Sorting Algorithms**:
    - Sorting is a common problem in computer science.
    - Reasons for sorting: Alphabetical order, numeric order, ranking.
    - Example: Bubble Sort Algorithm for digits 0 through 9.
        1. Place digits in a list.
        2. Scan the list and compare adjacent items.
        3. If items are in the wrong order, flip them.
        4. Continue scanning and flipping until the list is sorted.
        5. Return to the beginning of the list and repeat until no flips are needed.
    - Bubble sort guarantees a sorted list but is not the most efficient algorithm.
- **Efficiency of Algorithms**:
    - An algorithm must complete and provide the correct answer.
    - Efficiency is crucial, especially with large data sets.
    - Just because an algorithm works doesn't mean it's the best choice.
    - Bubble sort is not the fastest sorting algorithm; there are more efficient methods.

# Memory and Data Structures

1. **Introduction to Data Structures**:
    - Data structures allow efficient storage and retrieval of data.
    - Critical in managing large data sets, such as those in genomics.
2. **Genomic Data Storage**:
    - Genomic data often comes as long strings of characters (A, C, G, T).
    - Computers are adept at storing text, but efficiency can be improved.
3. **Efficient Storage Methods**:
    - When dealing with multiple sequences, store commonalities and differences to save space.
    - Efficient data structures help in quickly finding specific sequences within large data sets.
4. **Example of Efficient Data Storage**:
    - For a sequence of 100 nucleotides within a 3 billion base pair genome, use tags for chromosome and start location.
    - Store pointers to facilitate quick retrieval of sequences.
5. **Types of Data Structures**:
    - **Trees**: Organize data hierarchically.
    - **Lists**: Simple linear structures for storing sequences.
    - **Linked Lists**: Lists where elements point to the next element, facilitating easy insertion and deletion.
6. **Memory Addressing and Pointers**:
    - Each piece of memory has an address.
    - Pointers in programming point to these memory addresses, enabling efficient data retrieval.
7. **Efficiency in Data Structures**:
    - Representing DNA sequences efficiently can lead to significant space savings.
    - Standard text representation uses one byte (8 bits) per character.
    - DNA has only four letters (A, C, G, T), allowing for a more compressed representation using two bits per letter.
8. **Example of DNA Compression**:
    - A: 00, C: 01, G: 10, T: 11.
    - Fourfold compression achieved, reducing space from 8 bits to 2 bits per letter.
    - Important for handling large genomic data sets.
9. **Advanced DNA Representation**:
    - Capture patterns with biological functions, such as intron start (GT) and end (AG) sequences.
        - Intron: Genomumuzdaki genlerde bulunan ve aslında proteinleri kodlamayani, ancak DNA’dan RNA’ya ve protein geçiş sürecinde koparılan ve atılan kesintiye uğrayan dizilerdir.
    - Use probabilistic models to represent the likelihood of specific letters at certain positions.
    - Represent patterns visually using logos where letter height indicates probability.
10. **Conclusion**:
    - Efficient data structures are essential for managing large genomic data.
    - Proper representation and compression techniques can significantly optimize storage and retrieval processes.
    - Advanced models help capture biological patterns, aiding in further genomic analysis.

# Efficiency

- **Introduction to Efficiency**:
    - Efficiency is crucial in computer science, especially with big data.
    - Genomics provides an example of big data requiring efficient algorithms.
- **Example Scenario: Mail Delivery**:
    - Mail collection at various sites, centralized at a warehouse.
    - Simple but inefficient algorithm: Mailman picks up mail for one house, delivers it, and returns to the warehouse for the next house.
    - This method is inefficient due to excessive back-and-forth trips.
- **Improving Mail Delivery Efficiency**:
    - More efficient approach: Mailman picks up mail for multiple houses, delivers it sequentially, and minimizes trips back to the warehouse.
    - Conceptual analogy to the **Traveling Salesman Problem**:
        - Objective: Optimize the route to deliver mail to multiple houses efficiently.
        - Factors: Maximize truck capacity, minimize distance traveled, and deliver as much mail as possible before returning to the warehouse.
- **Traveling Salesman Problem (TSP)**:
    - Class of problems in algorithmic efficiency.
    - Goal: Find the shortest possible route that visits a set of locations and returns to the starting point.
    - Application to mail delivery: Optimize the route to cover as many houses as possible with minimal travel.
- **Key Considerations in Algorithmic Efficiency**:
    - **Data Retrieval**: Minimize trips to memory to fetch data.
    - **Time Complexity**: Reduce the number of steps required to complete a task.
    - **Space Complexity**: Optimize the use of memory.
- **Analyzing and Optimizing Algorithms**:
    - Evaluate what the computer is doing at each step.
    - Identify redundant operations or excessive resource use.
    - Seek ways to perform tasks in fewer steps, less time, and with less memory usage.
- **Conclusion**:
    - Efficient algorithms are essential for handling large data sets, like those in genomics.
    - Optimization involves reducing computational resources while achieving the desired outcome.
    - Understanding and applying efficient algorithms can significantly enhance performance in various computational tasks.

# Software Engineering

1. **Importance of Software Engineering**:
    - Often overlooked but essential in computational data analysis.
    - Focus on reliability, case handling, and performance.
2. **Programming vs. Mathematics**:
    - Example equation: \( z = \frac{x}{y} \).
    - In programming, additional checks are necessary (e.g., ensuring \( y \neq 0 \)) to prevent crashes.
3. **Handling Unexpected Cases**:
    - Software must account for rare but possible scenarios, especially with large datasets.
    - Good engineering ensures reliability in computational biology programs.
4. **Understanding Genomic Software**:
    - Necessary to comprehend program operations, not just treat them as black boxes.
    - Lack of understanding can lead to confusion and errors in interpreting outputs.
5. **Example: RNA Editing**:
    - RNA editing involves occasional changes in nucleotides after transcription from DNA.
    - Rare phenomenon but significant for gene regulation.
6. **Detecting RNA Editing**:
    - Compare DNA and RNA sequences from the same individual.
    - Misalignment indicates potential RNA editing.
7. **Case Study on RNA Editing Discovery**:
    - Scientists used alignment software and found numerous RNA-DNA differences, suggesting new RNA editing mechanisms.
    - Generated excitement but also controversy.
8. **Verification of Findings**:
    - Importance of questioning the validity of detected differences.
    - Even a 99.999% accuracy can lead to significant errors in large datasets.
9. **Critical Message**:
    - Software engineering is vital for genomic software.
    - Even well-engineered software can have bugs and errors, especially with big data.
    - Always verify and understand software outputs before making conclusions.

# What is Computational Biology Software?

Computational biology software plays a crucial role in transforming raw genomic data into meaningful information that can be used to make biological discoveries and guide experiments. Here is a brief introduction to this field and the types of software involved:

### Types of Computational Biology Software

1. **Analysis Pipelines**:
    - **Definition**: A series of software tools that process raw data through various stages to produce interpretable results.
    - **Purpose**: To convert raw DNA sequence data into actionable biological insights.
    - **Example**: Analyzing raw DNA sequences to detect variations and phenotypic differences in individuals.
2. **Software for Specific Tasks**:
    - **Noise Reduction**: Tools that clean up raw data to remove noise.
    - **Sequence Assembly**: Programs that assemble short sequences into longer, continuous sequences.
    - **Comparative Analysis**: Tools that compare sequences against a reference genome or among samples.
    - **Visualization Tools**: Software like Galaxy that allows users to visualize genomic data and analysis results.

### Example Pipeline: RNA-seq Analysis

1. **RNA-seq**:
    - **Purpose**: To sequence RNA from cells and determine which genes are active.
    - **Applications**: Comparing gene expression between cell types, studying cancer cells, etc.
2. **Tuxedo Pipeline Components**:
    - **Bowtie**: Aligns RNA sequences to the human genome.
    - **TopHat**: Handles spliced alignments for RNA sequences spanning multiple exons.
    - **Cufflinks**: Assembles alignments into gene structures and quantifies their expression.
    - **Cuffdiff**: Compares gene expression levels between samples.
3. **Updated Tools**:
    - **Bowtie2**: Improved version of Bowtie.
    - **HISAT**: A faster alignment tool replacing TopHat.
    - **StringTie**: Supersedes Cufflinks for transcript assembly and quantification.
    - **Ballgown**: Used for differential expression analysis.

### Importance of Keeping Up-to-Date

- **Technological Advancements**: As sequencing technologies evolve, new software tools are developed to handle new types of data.
- **Accuracy and Relevance**: Using outdated software on new data types can lead to incorrect results, making it critical to stay informed about the latest tools and methodologies.

### Conclusion

Computational biology software is essential for processing and interpreting vast amounts of genomic data. It involves a range of tools and pipelines, each designed to address specific aspects of data analysis, from noise reduction and sequence alignment to expression quantification and visualization. Staying current with the latest software and technologies is crucial for accurate and meaningful biological research.
