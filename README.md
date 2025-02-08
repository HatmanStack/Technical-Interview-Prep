# Technical-Interview-Prep

## Table of Contents
- [Leadership](#Leadership-Principles-(LP)-Overview)
- [Languages](#languages)
- [Data Structures](#data-structures)
- [Algorithms](#algorithms)
- [Design Patterns For Object-Oriented](#Design-Patterns-For-Object-Oriented)
- [Databases](#Databases)
- [Row vs Columnar Data](#Row-vs-Columnar-Data)
- [Distributed Computing](#Distributed-Computing)
- [OS Design](#OS-Design)
- [Internet](#Internet)
- [Machine Learning](#Machine-Learning)
- [MicroService vs Monolith](#MicroService-vs-Monolith)
- [System Design](#system-design)
  - [Criteria for Successful System Design](#Criteria-for-Successful-System-Design)
- [Logical and Maintainable Code](#logical-and-maintainable-code)
  - [Before the Interview](#Before-the-Interview)
  - [Common Design Patterns](common-design-patterns)
  - [Unit Testing](#Unit-Testing)
  - [During the Interview](#During-the-Interview)
- [Competencies in Data Structures and Algorithm](#Competencies-in-Data-Structures-and-Algorithm)
  - [Practice Topics](#Practice-Topics)
- [Problem Solving](#Problem-Solving)
  - [Demonstrating Your Competency](#Demonstrating-Your-Competency)
- [Amazon Leadership Principles Overview](#Amazon-Leadership-Principles-Overview)

## Leadership Principles (LP) Overview
### Amazon Leadership Principles

- **Earn Trust**: Build trust through candid communication, self-awareness, and benchmarking against the best.
- **Deliver Results**: Consistently meet business objectives with quality and timeliness, rising above setbacks.
- **Customer Obsession**: Prioritize customer needs and work backward from there.
- **Ownership**: Embrace accountability beyond immediate roles and short-term results.
- **Invent and Simplify**: Foster innovation and simplify processes, avoiding "not invented here" biases.
- **Are Right, A Lot**: Make informed decisions with sound judgment and diverse viewpoints.
- **Learn and Be Curious**: Pursue continuous improvement and exploration of new ideas.
- **Hire and Develop the Best**: Identify and nurture top talent, cultivating leaders across the organization.
- **Insist on the Highest Standards**: Set and maintain high standards, ensuring quality in what is delivered.
- **Think Big**: Encourage bold, visionary thinking to drive impactful results.
- **Bias for Action**: Value prompt decision-making and calculated risks.
- **Frugality**: Deliver more with less, leveraging constraints to drive innovation.
- **Dive Deep**: Engage with details comprehensively and question when data and anecdotes don't align.
- **Have Backbone; Disagree and Commit**: Challenge decisions thoughtfully, then commit fully once resolved.
- **Strive to be Earth's Best Employer**: Enhance workplace diversity, safety, and performance through empathy and fun.
- **Success and Scale Bring Broad Responsibility**: Lead with humility, pursuing improvements for community benefit while leaving a positive impact.

### Assessing Leadership Principles

#### Behavioral-based Questions
- Use behavioral questions to explore past experiences, focusing on actions taken and lessons learned.
- Avoid brain teasers. Focus is on real-world decision-making and problem-solving.

#### Preparing for the Competency
- Reflect on significant professional moments and how they align with Leadership Principles.
- Have specific examples ready to demonstrate risk-taking, success, failure, and growth.
- Embrace failure as part of the innovative process, highlighting learnings and iterations.

### STAR Method for Examples

- **Situation**: Clearly set the context of a specific event or challenge. Include enough detail for understanding complexities.
  - Example: "During a crucial product launch with tight deadlines, our team encountered unexpected supply chain disruptions."

- **Task**: Define the goal or task you were aiming to achieve. Discuss both qualitative and quantitative objectives.
  - Example: "As project lead, my task was to ensure the product launched on time, meeting quality and cost targets."

- **Action**: Detail the specific actions you took to address the situation. Use "I" to focus on your contributions.
  - Example: "I analyzed alternative suppliers, negotiated terms, and adjusted the project scope to mitigate delays."

- **Result**: Highlight the outcomes of your actions, any trade-offs, and what you learned.
  - Example: "The product launched as scheduled with a 10% cost reduction, which improved market share. The experience taught me about resilient supply chain solutions."

### Quantifying Results
- **Metrics Examples**:
  - Cost savings, revenue generation
  - Volume, size, scale quantification
  - Percentage improvements or year-over-year growth
  - Time to market, implementation time reductions
  - Quality improvements impacting customers or teams
<br>[Top](#table-of-contents)

## Languages
### Python 3
- **Memory Management**: Uses automatic garbage collection, with reference counting and cyclic garbage collector.
- **Collections**: Common ones are `list`, `dict`, `set`, and `tuple`. The `collections` module provides specialized types like `deque`, `Counter`, `OrderedDict`.
- **Libraries**: Extensive standard library and third-party packages available through PyPI. Common libraries include `requests` for HTTP requests, `pandas` for data manipulation, and `numpy` for numerical computing.
- **Syntax**: Indentation is crucial. Supports multiple assignment, list comprehensions, and has powerful string manipulation capabilities with f-strings.

### Java 8
- **Memory Management**: Managed via the JVM with garbage collection. Enhancements like the G1 garbage collector were introduced.
- **Libraries**: Rich standard API, with libraries like `java.util` for collections (e.g., `ArrayList`, `HashMap`) and `java.time` for dealing with date and time.
- **Features**: Introduced lambda expressions, the Streams API for functional-style operations over collections, `Optional` class for better handling of nulls.
- **Concurrency**: Strong concurrency utilities in `java.util.concurrent` package.

### JavaScript
- **Memory Management**: Mostly automatic with garbage collection, but care needed with closures to avoid memory leaks.
- **Collections**: Arrays, objects, and newer additions like `Map` and `Set`.
- **Libraries and Frameworks**: Diverse ecosystem, with popular libraries like React, Angular, and libraries like Lodash for utility functions.
- **Features**: Asynchronous programming is handled via callbacks, promises, and `async/await`. Prototypes are core to object inheritance.
<br> [Top](#table-of-contents)

## Data Structures
### Arrays
- **Usage**: Best for indexed access where elements are stored contiguously.
- **Operations**: Access O(1), search O(n), insertion/deletion O(n).
- **Memory**: Fixed-size in static arrays, flexible in dynamic arrays like Python lists.

### Linked Lists
- **Usage**: Useful when frequent insertions and deletions are needed.
- **Types**: Singly linked (single pointer to next node) and doubly linked (pointers to both next and previous nodes).
- **Operations**: Insertion/deletion O(1) at head, searching O(n).
- **Memory**: Overhead due to pointers.

### Stacks
- **Usage**: Suitable for LIFO (Last In, First Out) operations, e.g., backtracking algorithms.
- **Operations**: Push/pop O(1).
- **Memory**: Based on underlying data structure (array or linked list).

### Queues
- **Usage**: Suitable for FIFO (First In, First Out) operations, e.g., task scheduling.
- **Types**: Simple queue, double-ended queue (deque), and priority queue.
- **Operations**: Enqueue/dequeue O(1) for basic queues.
- **Memory**: Similar to stacks.

### Hash Tables
- **Usage**: Fast key-based access.
- **Operations**: Average O(1) for insert, search, and delete; worst-case O(n).
- **Memory**: Can be memory-intensive due to potential need for resizing.

### Trees
- **Types**: Binary trees, binary search trees, AVL trees, red-black trees.
- **Usage**: Hierarchical data storage, like file systems and databases.
- **Operations**: Vary by type, with BST operations (insert, find, delete) typically O(log n) when balanced.
- **Memory**: Depends on tree type, additional pointers for tree navigation.

### Graphs
- **Types**: Directed/undirected, weighted/unweighted, represented using adjacency matrix or list.
- **Usage**: Networks and relationships modeling, like social networks.
- **Operations**: Varies widely; traversing via BFS or DFS takes O(V + E), where V is vertices and E is edges.
- **Memory**: Space depends on representation; adjacency matrix O(V^2), adjacency list O(V + E).

### Heaps
- **Types**: Min-heap and max-heap.
- **Usage**: Priority queue implementation.
- **Operations**: Insert O(log n), extract-min/max O(log n).
- **Memory**: Typically an array, efficient in terms of storage.
<br> [Top](#table-of-contents)

## Algorithms
### Traversals
- **Tree Traversals**: 
  - In-order, pre-order, post-order for binary trees.
  - Common scenarios include tree construction and evaluation of expressions.

- **Graph Traversals**: 
  - Breadth-First Search (BFS): Uses a queue, explores level by level, suitable for shortest path problems in unweighted graphs.
  - Depth-First Search (DFS): Uses a stack or recursion, explores as far as possible along each branch, useful for connectivity and pathfinding in mazes.

### Divide and Conquer
- **Concept**: Breaking a problem into smaller subproblems, solving them independently, and combining their solutions.
- **Applications**: 
  - Merge Sort (O(n log n)): Splits array and merges sorted halves.
  - Quick Sort (average O(n log n), worst-case O(n^2)): Partition-based approach, efficient on average with good pivot selection.
  - Binary Search (O(log n)): Efficient search in sorted arrays/lists.

### Algorithm Analysis
- **Time Complexity**: Analyzing how the runtime increases with input size; e.g., linear (O(n)), logarithmic (O(log n)), quadratic (O(n^2)).
- **Space Complexity**: Understanding additional memory usage; e.g., recursive algorithms can have higher space complexity due to stack usage.

### Trade-Offs
- **BFS vs. DFS**: 
  - BFS finds the shortest path in unweighted graphs, but is memory-intensive; DFS is memory efficient and easier to implement recursively but doesn't guarantee shortest path without modifications (like iterative deepening).
- **Divide and Conquer**: Generally efficient but may have overhead in dividing and combining stages, such as in merge sort.
<br> [Top](#table-of-contents)

## Design Patterns For Object-Oriented
### Object-Oriented Design Principles
- **Encapsulation**: Hiding the internal state and requiring all interaction through an interface. This reduction in coupling helps ensure that modifying one part of the system doesn't inadvertently affect other parts.

- **Abstraction**: Simplifying complex systems by modeling classes based on the essential qualities for a specific purpose, which enhances code clarity and reuse.

- **Inheritance**: Facilitating code reuse by creating a new class based on an existing class. It's crucial to use this judiciously to avoid tight coupling or complexity.

- **Polymorphism**: Allowing entities to take on multiple forms. This is often seen in the ability to call the same method on different objects and have each of them respond differently, aiding in flexible and scalable code design.

### Common Design Patterns
- **Creational Patterns**:
  - *Singleton*: Ensures a class has only one instance and provides a global access point to it.
  - *Factory Method*: Provides an interface for creating objects, but lets subclasses alter the type of objects that will be created.

- **Structural Patterns**:
  - *Adapter*: Allows incompatible interfaces to work together by acting as a bridge.
  - *Decorator*: Adds behavior to objects dynamically without modifying their structure.

- **Behavioral Patterns**:
  - *Observer*: Establishes a subscription mechanism to allow multiple objects to listen and react to events or changes in another object.
  - *Strategy*: Defines a family of algorithms, encapsulates each one, and makes them interchangeable to let the algorithm vary independently from clients that use it.

### Defending Your Design Choices
When discussing your design choices:
- **Justify Extensibility**: How does your design accommodate future changes or extensions without requiring significant rework?
- **Highlight Maintainability**: How do the chosen patterns and principles reduce complexity and prevent potential bugs?
- **Scalability**: How does your design ensure performance will remain efficient as load and usage increase?
- **Trade-Offs**: Be prepared to discuss potential downsides or trade-offs made in your design choices, such as increased complexity for extra functionality.
<br> [Top](#table-of-contents)

## Databases
### Relational Databases
- **Structure**: Data is organized into tables with rows and columns, following a strict schema.
- **Relationships**: Employ foreign keys to maintain relationships between tables.
- **Transactions**: Support ACID (Atomicity, Consistency, Isolation, Durability) properties, ensuring reliable transactions.
- **Use Cases**: Ideal for complex queries and transactions, where data integrity and relationships are crucial, such as financial systems.

### Non-Relational Databases (NoSQL)
- **Flexibility**: Allow for varied data storage models, including document, key-value, column-family, and graph stores.
- **Scalability**: Generally offer horizontal scalability, making them well-suited for large-scale distributed environments.
- **Trade-Offs**: Often sacrifice some ACID properties, using eventual consistency models to enhance performance and availability.
- **Use Cases**: Ideal for large volumes of unstructured or semi-structured data, real-time analytics, and flexible schema requirements, such as social media platforms, IoT, and content management systems.

### Examples of Non-Relational Databases
- **Document Store**: MongoDB, CouchDB. Stores data in JSON-like documents, providing flexibility and hierarchical storage.
- **Key-Value Store**: DynamoDB, Redis. Stores simple key-value pairs, ideal for caching and simple lookup use cases.
- **Column-Family Store**: Cassandra, HBase. Optimized for queries over large datasets, where columns are distributed across multiple servers.
- **Graph Store**: Neo4j. Focuses on relationships and graphs, suitable for network and recommendation engines.

### Trade-Offs

- **Consistency vs. Availability vs. Partition Tolerance** (CAP Theorem):
  - **Consistency**: Ensures every read receives the latest write (e.g., important for financial systems).
  - **Availability**: Guarantees a response to every request, even if the data isn't the latest (e.g., social networks).
  - **Partition Tolerance**: Operates despite network failures, crucial for distributed systems.

- **Schema Flexibility**:
  - **Relational Databases**: Offer rigidity with enforced relationships and data integrity, but changing schemas is complex.
  - **Non-Relational Databases**: Provide flexibility for evolving data models by allowing unstructured data, sacrificing enforced constraints.

- **Query Complexity**:
  - **Relational Databases**: Excel in handling complex queries with SQL, offering robust query optimization.
  - **Non-Relational Databases**: Require custom query solutions for complex operations, which might demand more development effort.
<br> [Top](#table-of-contents)

## Row vs Columnar Data
### Row-Oriented Storage
- **Design**: Stores all columns of a single row together.
- **Optimized For**: Transactional environments where operations often involve the entire row. Insertions, updates, and deletes are efficient because they affect localized areas on disk.
- **Trade-Off**: Retrieval of many rows is fast, but accessing specific columns across many rows (like aggregations or analytics) is less efficient because of non-sequential disk access and additional I/O.

### Columnar (Column-Oriented) Storage
- **Design**: Stores each column's data separately.
- **Optimized For**: Analytical queries, such as aggregations or selecting specific columns across many rows, allowing efficient compression and I/O since only relevant columns need to be read.
- **Trade-Off**: Writing or modifying data is less efficient since it may require updates to multiple locations, and transaction processing can be slower due to scattered data.

### Correlation to BFS vs. DFS
- **BFS (Breadth-First Search)**:
  - **Similarity with Row Storage**: Just as BFS explores all nodes level by level, row storage retrieves full rows comprehensively, making it effective for operations where context (entire row) is necessary.
  - **Trade-Off**: Can require lots of memory or I/O if a large number of rows are processed without need for full depth detail, similar to BFS needing to track full levels.

- **DFS (Depth-First Search)**:
  - **Similarity with Columnar Storage**: DFS is akin to drilling down a single path (or column) deeply before branching out, maximizing efficient retrieval of related nodes (or data points within a column).
  - **Trade-Off**: May miss contextual depth for full rows, akin to DFS missing breadth exploration initially, requiring backtracking or additional queries.
<br> [Top](#table-of-contents)

## Distributed Computing
### Service-Oriented Architectures (SOA)
- **Concept**: An architectural pattern where services are provided to other components by application components through a network, typically using a set of protocols.
- **Benefits**: Encourages reusability, scalability, and separation of concerns. Each service can be developed and deployed independently.
- **Challenges**: Involves complexities such as service discovery, load balancing, and failure handling.

### Map-Reduce
- **Concept**: A programming model for processing and generating large data sets with a parallel, distributed algorithm on a cluster.
- **Process**: Consists of two key functions: Map (filters and sorts) and Reduce (aggregates and reduces the results from the map function).
- **Applications**: Particularly useful for tasks involving large-scale data processing across distributed nodes, like indexing, log analysis, and data mining.

### Distributed Caching
- **Concept**: Stores data in a cache across multiple servers or nodes to increase speed and efficiency of data retrieval.
- **Benefits**: Reduces database load, decreases latency, and improves data retrieval performance.
- **Challenges**: Maintaining consistency and dealing with cache invalidation across distributed nodes.

### Load Balancing
- **Concept**: A method of distributing incoming network traffic across multiple servers to ensure no single server is overwhelmed.
- **Benefits**: Increases availability and reliability, optimizes resource use, ensures scalability, and provides failover.
- **Techniques**: Includes round-robin, least connections, IP hash, and others.

### Other Concepts
- **Fault Tolerance**: Designing systems to continue operating properly in the event of failures, through redundancy and replication.
- **Consistency Models**: Understanding weak, strong, and eventual consistency to manage data integrity in distributed systems.
- **Scalability**: Ability to handle growth by adding resources, either vertically (adding more power to the existing machines) or horizontally (adding more machines to the pool).
<br> [Top](#table-of-contents)

## OS Design
### Memory Management
- **Concept**: Memory management is the process of controlling and coordinating computer memory, assigning portions to various running programs to optimize overall system performance.
- **Memory Leaks**: Occur when a program consumes memory without eventually freeing it, leading to reduced available memory over time.
- **Dynamic Allocation**: Allocates memory at runtime as needed, allowing programs to use memory more flexibly.
- **Garbage Collection**: An automatic memory recovery process that identifies and reclaims unused memory to prevent leaks.
- **Stack vs. Heap Management**: Memory is divided into stack (for static memory allocation) and heap (for dynamic memory allocation); efficient management of these areas is crucial for applications.

### Processes and Threads
- **Processes**: Self-contained execution environments that include their own memory space; they represent individual programs in action on a computer.
- **Context Switching**: The process of storing and restoring the state of a CPU so that process execution can be resumed from the same point at a later time; it's a key overhead in managing processes.
- **Inter-process Communication (IPC)**: Mechanisms allowing processes to communicate and synchronize their actions when processes are isolated.
- **Threads**: Smaller units of tasks that belong to a process; they operate within the same memory space and are therefore lighter and faster to switch between than processes.

### Synchronization
- **Concept**: Synchronization involves managing access to shared resources between threads or processes to prevent simultaneous access that can lead to errors.
- **Race Conditions**: Occur when multiple threads or processes attempt to change a shared resource concurrently, leading to unexpected behavior.
- **Locks and Mutexes**: Tools to enforce exclusive access to a resource, ensuring only one thread can use it at a time.
- **Semaphores**: Synchronization tools that control access based on counting, allowing multiple accesses up to a defined limit.
- **Monitors**: High-level synchronization constructs that combine functionality of locks and condition variables.

### Paging
- **Concept**: Paging is a system where the computer's memory is divided into fixed-size pages, helping eliminate the need to allocate physical memory contiguously and optimizing memory use.
- **Page Faults**: Occur when a program tries to access data not currently mapped to physical memory, causing a delay as the data is fetched from storage.
- **Thrashing**: A condition where constant page faults significantly reduce system performance due to excessive paging activities.

### Multithreading
- **Concept**: Multithreading is running multiple threads in parallel within a process, enabling concurrent execution of tasks for performance gains.
- **Efficiency and Responsiveness**: Threads can perform tasks independently and concurrently, making applications more efficient and responsive, especially on systems with multiple processors.
- **Thread Contention**: Occurs when multiple threads attempt to use the same resource simultaneously, potentially leading to performance bottlenecks.
- **Deadlocks**: Situations where two or more threads wait indefinitely for resources locked by each other, preventing further execution.
<br> [Top](#table-of-contents)

## Internet
### DNS (Domain Name System)
- **Function**: Translates human-readable domain names (like www.amazon.com) into IP addresses that computers can understand.
- **Process**: When a browser requests a web page, it first queries the DNS server to resolve the domain name to an IP address.

### TCP/IP (Transmission Control Protocol/Internet Protocol)
- **TCP**: Provides reliable, ordered, and error-checked delivery of data between applications. It's a connection-oriented protocol ensuring all packets arrive correctly.
- **IP**: Responsible for addressing and routing packets between devices. It ensures data packets find their way across networks to reach their intended destination.

### HTTP/HTTPS
- **HTTP**: The protocol used for transferring web pages on the internet. HTTP requests and responses are the primary means for browsers and servers to communicate.
- **HTTPS**: An extension of HTTP securing data exchange with SSL/TLS, which encrypts data for secure transmission.

### Socket Connections
- **Function**: Enable communication between a client and server over a network. Sockets use protocols like TCP to establish a direct link for data exchange.
- **Usage**: Web servers and clients open sockets to interact, sending and receiving data much like a phone call's open line.

### The Browser’s Role
1. **Request Initiation**: User enters a URL, triggering an HTTP request from the browser.
2. **DNS Resolution**: Browser queries DNS to obtain an IP address for the domain.
3. **Connection Establishment**: A TCP connection is established with the server using the IP address and a specific port (usually 80 for HTTP and 443 for HTTPS).
4. **Data Transfer**: The browser sends an HTTP request to the server, which responds with the content (HTML, CSS, JS, images) to be displayed.
5. **Rendering**: The browser parses and renders the response content, displaying the web page to the user.

### Additional Concepts
- **Caching**: Web browsers cache resources to reduce load times on subsequent requests.
- **Cookies**: Small pieces of data stored by the browser to track stateful information and sessions.
<br> [Top](#table-of-contents)

## Machine Learning
### Problem Formulation
- **Define the Problem**: Translate the business objective into a machine learning task, such as classification, regression, clustering, or recommendation.
- **Identify Outputs**: Determine what predictions or insights are required.
- **Data Sources**: Identify and gather data that is relevant to the problem. Consider structured databases, text, images, or other sources.

### Data Annotation and Preparation
- **Annotation**: If using supervised learning, ensure data is labeled. Employ techniques like crowdsourcing or expert annotation.
- **Cleaning and Preprocessing**: Handle missing values, outliers, normalization, and feature engineering.
- **Splitting Data**: Divide data into training, validation, and test sets to ensure unbiased evaluation of models.

### Modeling Approaches
- **Algorithm Selection**: Choose a suitable algorithm based on the problem type, available data, and computational resources. Options include:
  - Linear Regression, Decision Trees for simple problems.
  - Support Vector Machines, Random Forests, or Neural Networks for complex, high-dimensional data.
- **Model Training**: Train models using the training dataset while tuning hyperparameters to optimize performance.
- **Evaluation Metrics**: Choose appropriate metrics such as accuracy, precision, recall, F1-score for classification, or RMSE for regression.

### Error Analysis and Evaluation
- **Test Protocols**: Use cross-validation to assess model generalization.
- **Error Analysis**: Examine incorrectly predicted instances to gain insights into model weaknesses and data issues.
- **Statistical Significance**: Validate if the observed performance improvements are statistically significant, using techniques like bootstrapping or hypothesis testing.

### Potential Pitfalls
- **Overfitting**: Ensure the model isn't too complex relative to the size of the data, using regularization or pruning techniques.
- **Bias and Variance**: Balance bias and variance; high bias indicates underfitting, while high variance indicates overfitting.
- **Data Leakage**: Ensure no information from the test set leaks into the training process, maintaining the integrity of evaluation.
<br> [Top](#table-of-contents)

## MicroService vs Monolith
### Monolithic Architecture
- **Design**: A single unified codebase where all modules are tightly coupled and executed as a single application.
  
#### Benefits:
- **Simplicity**: Easier to develop and test, especially for smaller teams or projects.
- **Performance**: Direct function calls within a single process can be faster compared to inter-service communication.
- **Deployment**: Single deployment unit simplifies the deployment process.

#### Trade-Offs:
- **Scalability**: Difficult to scale specific components since the entire application must scale.
- **Flexibility**: Slower to adopt new technologies as changes affect the entire application.
- **Maintenance**: As the application grows, it can become complex and harder to manage.

### Microservices Architecture
- **Design**: Composed of small, independent services, each focused on a specific business function and able to be deployed individually.

#### Benefits:
- **Scalability**: Services can be scaled independently based on demand.
- **Flexibility**: Allows the use of different technologies or languages for different services.
- **Resilience**: Failures in one service don’t necessarily cascade to others, improving fault tolerance.
- **Deployment**: Enables continuous delivery and rapid deployment of individual services.

#### Trade-Offs:
- **Complexity**: Managing a distributed system with numerous services can be complex.
- **Communication Overhead**: Inter-service communication over the network can introduce latency and requires careful management.
- **Data Consistency**: Maintaining consistency across services can be challenging.
<br> [Top](#table-of-contents)

## System Design
### Core Concepts
- **Scalability and Maintainability**: Design systems to be scalable and maintainable, even under massive, unpredictable environments like those at Amazon. Understand how distributed systems, SOA, and n-tier architectures contribute to robust design.
- **Object-Oriented Design Principles**: Use these principles to build extensible and bug-free software components.
- **Black Box Design**: Focus on designing systems that function effectively as a unit, abstracting internal complexities while ensuring deployment, scaling, and availability are prioritized.

### Assessing System Design
- **Clarifying Requirements**: Start by asking clarifying questions to define the user's needs and scope down the system requirements. Consider user expectations, potential growth, and the system's problem-solving aims.
- **Design Framework**: Develop a systematic approach for black box design that addresses deployment, scaling, failures, availability, and performance. Incorporate latency and concurrency considerations in your discussions.

### Preparing for the Competency
### Key Topics to Review
- **Software Components**: Familiarize yourself with components like databases (SQL, NoSQL), application servers, and monitoring tools. Example: Understand when to use relational vs. non-relational databases based on data structure and access patterns.
- **Distributed Systems and SOA**: Review concepts such as microservices, service orchestration, and inter-service communication protocols (e.g., REST, gRPC). Example: An e-commerce platform using microservices for inventory, payments, and user management with APIs for communication.
- **N-tier Architecture**: Dive into the separation of concerns between presentation, application logic, and data storage layers. Example: A 3-tier web application that uses front-end (UI), application (business logic), and database tiers to manage complexity and scalability.
- **Diagramming and Whiteboarding**: Practice sketching designs to communicate system architecture visually. Example: Use sequence diagrams to represent the flow of user requests from the front-end to the back-end, illustrating interactions between components.
<br>[Top](#table-of-contents)

### Criteria for Successful System Design
#### Create a Comprehensive Design

- **Requirement Fulfillment**: Example: If designing a social media application, your system should address constraints like data privacy, user scalability, and real-time updates. Explicitly mention assumptions, such as peak concurrent users or data retention policies.

- **Scalability and Core Functionality**: Design a system capable of handling growth, such as implementing load balancers to distribute traffic across application servers. Example: A video streaming platform that adapts to a spike in viewers with autoscaling and CDN integration.

- **Best Practices**: Stay informed about the best practices in your chosen tech stack. Example: For a cloud-native application, leverage services like AWS Lambda for serverless computing to optimize resource usage and costs.

#### Design for Operational Performance

- **Metrics and Monitoring**: Example: Implement dashboards using tools like Prometheus and Grafana to monitor CPU usage, response times, and error rates. Define metrics that help identify issues proactively.

- **Failure Planning and Resilience**: Consider redundancy methods like database replication and failover strategies. Example: For a financial application, design for immediate failover to backup systems to minimize downtime during outages.

- **Debugging and Logging**: Establish centralized logging (e.g., ELK stack) and fine-grained logs to aid in identifying and troubleshooting issues quickly.

#### Identify Potential Shortcomings and Tradeoffs

- **Performance vs. Cost**: Example: Choosing between a high-performance, costlier solution like all-SSD storage versus a budget-friendly HDD setup for a non-critical app. Discuss how user demands and operational priorities inform this choice.

- **Fault Tolerance vs. Complexity**: Implementing distributed data processing across multiple regions can offer fault tolerance but adds system complexity and coordination challenges. Discuss the tradeoff between increased reliability and operational complexity.

- **Single Point of Failure (SPOF)**: Identify SPOFs and propose redundancy plans, such as using multiple load balancers or geographic DNS routing. Evaluate tradeoffs involved in eliminating SPOFs, such as increased cost or latency.

### Important System Design Considerations

- **Scaling**: Consider horizontal and vertical scaling techniques. Example: Use database sharding to horizontally scale data storage for an application with a large dataset, ensuring each shard has its own capacity limits.

- **Caching**: Implement caching strategies (e.g., Redis, Memcached) to reduce latency and database load. Example: A news website caching popular articles using a distributed cache to enhance load times.

- **Load Balancing**: Use load balancing to manage user requests across multiple servers efficiently. Example: Deploying an application across AWS EC2 instances using Elastic Load Balancing to ensure equal distribution of traffic.

- **Microservices and Sharding**: Design systems with microservices to decouple functionalities for easier scaling and maintenance. Utilize sharding for distributed databases to handle large volumes of data.

- **Fault Tolerance and Redundancy**: Plan for redundancy in critical systems components to maintain service continuity during failures. Example: Multi-AZ deployments in cloud services to ensure high availability.

Note: Effective system design integrates robust architecture, thought-out tradeoffs, and scalability considerations, ensuring the system meets current demands and can grow with future requirements.
<br>[Top](#table-of-contents)

## Logical and Maintainable Code
### Core Concepts
- Break down complex problems into smaller, focused functions
- Use classes to encapsulate related functionality
- Implement inheritance and interfaces for extensible designs
- Separate concerns into distinct modules/components
- Follow single responsibility principle
- Create clear hierarchies of functionality

### Naming Conventions
- Use descriptive variable names that indicate purpose
- Choose method names that describe actions
- Name classes based on their responsibilities
- Avoid abbreviations unless universally understood
- Use consistent naming patterns throughout codebase
- Include units in variable names when applicable (e.g., timeoutSeconds)

### Documentation and Readability
- Write self-documenting code when possible
- Include purpose-focused comments for complex logic
- Document public APIs and interfaces
- Use consistent indentation and formatting
- Group related code together
- Leave spaces between logical sections
- <br> [Top](#table-of-contents)

### Before the Interview
SOLID Principles in Python<br>
Single Responsibility Principle (SRP)
```# Bad
class User:
    def __init__(self, name: str):
        self.name = name
    
    def save_to_db(self):  # Database logic shouldn't be in User class
        pass
    
    def generate_report(self):  # Reporting shouldn't be in User class
        pass

# Good
class User:
    def __init__(self, name: str):
        self.name = name

class UserRepository:
    def save(self, user: User):
        pass

class UserReporter:
    def generate_report(self, user: User):
        pass
```
Open/Closed Principle (OCP)
```
# Bad
class PaymentProcessor:
    def process_payment(self, payment_type: str):
        if payment_type == "credit":
            # process credit payment
            pass
        elif payment_type == "debit":
            # process debit payment
            pass

# Good
from abc import ABC, abstractmethod

class PaymentProcessor(ABC):
    @abstractmethod
    def process_payment(self):
        pass

class CreditPaymentProcessor(PaymentProcessor):
    def process_payment(self):
        # process credit payment
        pass

class DebitPaymentProcessor(PaymentProcessor):
    def process_payment(self):
        # process debit payment
        pass
```
Liskov Substitution Principle (LSP)
```
# Bad
class Bird:
    def fly(self):
        pass

class Penguin(Bird):  # Penguins can't fly!
    def fly(self):
        raise Exception("Can't fly")

# Good
class Bird:
    def move(self):
        pass

class FlyingBird(Bird):
    def fly(self):
        pass

class SwimmingBird(Bird):
    def swim(self):
        pass
```
Interface Segregation Principle (ISP)
```
# Bad
class Worker:
    def work(self):
        pass
    def eat(self):
        pass
    def sleep(self):
        pass

# Good
class Workable:
    def work(self):
        pass

class Eatable:
    def eat(self):
        pass

class Human(Workable, Eatable):
    def work(self):
        pass
    def eat(self):
        pass
```
Dependency Inversion Principle (DIP)
```
# Bad
class EmailSender:
    def send_email(self):
        pass

class NotificationService:
    def __init__(self):
        self.email_sender = EmailSender()  # Direct dependency

# Good
class MessageSender(ABC):
    @abstractmethod
    def send_message(self):
        pass

class EmailSender(MessageSender):
    def send_message(self):
        pass

class NotificationService:
    def __init__(self, message_sender: MessageSender):
        self.message_sender = message_sender  # Dependency injection
```
<br> [Top](#table-of-contents)
### Common Design Patterns
Creational Patterns<br>
Singleton
```
class Singleton:
    _instance = None
    
    def __new__(cls):
        if cls._instance is None:
            cls._instance = super().__new__(cls)
        return cls._instance
```
Factory Method
```
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def speak(self):
        pass

class Dog(Animal):
    def speak(self):
        return "Woof!"

class Cat(Animal):
    def speak(self):
        return "Meow!"

class AnimalFactory:
    def create_animal(self, animal_type: str) -> Animal:
        if animal_type == "dog":
            return Dog()
        elif animal_type == "cat":
            return Cat()
```
Structural Patterns<br>
Adapter
```
class OldSystem:
    def old_operation(self):
        return "old operation"

class NewSystem:
    def new_operation(self):
        return "new operation"

class SystemAdapter(OldSystem):
    def __init__(self, new_system: NewSystem):
        self.new_system = new_system
    
    def old_operation(self):
        return self.new_system.new_operation()
```
Decorator
```
from functools import wraps

def log_execution(func):
    @wraps(func)
    def wrapper(*args, **kwargs):
        print(f"Executing {func.__name__}")
        result = func(*args, **kwargs)
        print(f"Finished {func.__name__}")
        return result
    return wrapper

@log_execution
def example_function():
    pass
```
Behavioral Patterns<br>
Observer
```
class Subject:
    def __init__(self):
        self._observers = []
        self._state = None

    def attach(self, observer):
        self._observers.append(observer)

    def notify(self):
        for observer in self._observers:
            observer.update(self._state)

class Observer(ABC):
    @abstractmethod
    def update(self, state):
        pass
```
Strategy
```
from abc import ABC, abstractmethod

class SortStrategy(ABC):
    @abstractmethod
    def sort(self, data: list) -> list:
        pass

class QuickSort(SortStrategy):
    def sort(self, data: list) -> list:
        # Implementation
        pass

class MergeSort(SortStrategy):
    def sort(self, data: list) -> list:
        # Implementation
        pass

class Sorter:
    def __init__(self, strategy: SortStrategy):
        self.strategy = strategy

    def sort(self, data: list) -> list:
        return self.strategy.sort(data)
```
<br> [Top](#table-of-contents)
### Unit Testing
```
import unittest
from decimal import Decimal
from typing import List

class ShoppingCart:
    def __init__(self):
        self.items: List[dict] = []
    
    def add_item(self, name: str, price: Decimal):
        self.items.append({"name": name, "price": price})
    
    def calculate_total(self) -> Decimal:
        return sum(item["price"] for item in self.items)
    
    def apply_discount(self, percentage: int) -> Decimal:
        if not 0 <= percentage <= 100:
            raise ValueError("Discount must be between 0 and 100")
        total = self.calculate_total()
        discount = total * (Decimal(percentage) / 100)
        return total - discount

class TestShoppingCart(unittest.TestCase):
    def setUp(self):
        self.cart = ShoppingCart()
    
    def test_empty_cart_total(self):
        self.assertEqual(self.cart.calculate_total(), Decimal('0'))
    
    def test_adding_items(self):
        self.cart.add_item("book", Decimal('10.00'))
        self.cart.add_item("pen", Decimal('5.00'))
        self.assertEqual(self.cart.calculate_total(), Decimal('15.00'))
    
    def test_apply_valid_discount(self):
        self.cart.add_item("laptop", Decimal('1000.00'))
        discounted_total = self.cart.apply_discount(10)
        self.assertEqual(discounted_total, Decimal('900.00'))
    
    def test_invalid_discount_raises_error(self):
        with self.assertRaises(ValueError):
            self.cart.apply_discount(101)
```
Testing with Mocks
```
from unittest.mock import Mock, patch
import requests

class UserService:
    def __init__(self, api_url: str):
        self.api_url = api_url
    
    def get_user(self, user_id: int) -> dict:
        response = requests.get(f"{self.api_url}/users/{user_id}")
        if response.status_code == 404:
            raise ValueError("User not found")
        return response.json()

class TestUserService(unittest.TestCase):
    def setUp(self):
        self.service = UserService("http://api.example.com")
    
    @patch('requests.get')
    def test_get_existing_user(self, mock_get):
        # Setup mock
        mock_response = Mock()
        mock_response.status_code = 200
        mock_response.json.return_value = {"id": 1, "name": "John Doe"}
        mock_get.return_value = mock_response
        
        # Test
        user = self.service.get_user(1)
        self.assertEqual(user["name"], "John Doe")
        mock_get.assert_called_with("http://api.example.com/users/1")
    
    @patch('requests.get')
    def test_get_nonexistent_user(self, mock_get):
        # Setup mock
        mock_response = Mock()
        mock_response.status_code = 404
        mock_get.return_value = mock_response
        
        # Test
        with self.assertRaises(ValueError):
            self.service.get_user(999)
```
### Testing Best Practices Demonstrated:
- Use descriptive test names
- One assertion per test when possible
- Proper setup and teardown
- Testing edge cases and exceptions
- Using mocks for external dependencies
- Parameterized testing for multiple cases
- Testing both valid and invalid inputs
- Clear separation of test cases

### Practice Breaking Down Complex Problems
- Identify the core functionality
- Separate concerns into modules
- Define interfaces between components
- Apply appropriate design patterns
- Follow SOLID principles
- Write unit tests for each component

### Code Style Guidelines
- Follow PEP 8 for Python
- Use meaningful variable and function names
- Keep functions small and focused
- Write docstrings for public interfaces
- Use type hints for better readability
- Maintain consistent indentation
- Group related functionality
- Comment complex algorithms
- <br> [Top](#table-of-contents)

### During the Interview
- Gather requirements before coding
- Discuss approach with interviewer
- Start with simple working solution
- Use clear naming conventions
- Break functionality into logical components
- Consider edge cases
- Think about future maintainability

### Common Pitfalls to Avoid
- Writing monolithic functions
- Using unclear variable names
- Copying/pasting code instead of refactoring
- Over-engineering simple solutions
- Ignoring error handling
- Writing untestable code
- Making assumptions without clarifying requirements

### Best Practices
- Write code for future maintainers
- Keep functions focused and small
- Use consistent formatting
- Handle errors appropriately
- Make code changes easy to trace
- Design for extensibility
- Follow language conventions
- Consider performance implications

### Review Questions and Answers
Q: How would you refactor a large function into smaller, more manageable pieces?<br>
A: Start by identifying distinct responsibilities within the function. Extract similar operations into separate methods. Use meaningful names for new methods that describe their purpose. Ensure each method has a single responsibility. Pass necessary parameters and maintain proper error handling. Consider creating classes if methods share common data.<br><br>
Q: What naming conventions make code more maintainable?<br>
A: Use descriptive, action-based names for methods (e.g., calculateTotalPrice instead of calc). Include units in variable names (timeoutSeconds). Use consistent casing (camelCase for methods, PascalCase for classes). Avoid abbreviations unless standard. Name boolean variables with is/has prefix. Use domain-specific terminology consistently.<br><br>
Q: How do you handle new requirements without rewriting existing code?<br>
A: Follow Open/Closed Principle - extend functionality through inheritance or interfaces rather than modifying existing code. Use strategy pattern for varying behaviors. Implement facade pattern to hide complexity. Create abstract base classes for common functionality. Use dependency injection to swap implementations.<br><br>
Q: What makes code easy to test?<br>
A: Small, focused functions with single responsibilities. Pure functions without side effects. Dependency injection for external services. Clear input/output contracts. Proper exception handling. Minimal global state. Mock-friendly interfaces. Separate business logic from infrastructure code.<br><br>
Q: How do you balance simplicity with extensibility?<br>
A: Start with the simplest solution that works. Add abstraction layers only when needed for current requirements. Use interfaces to define clear contracts. Follow YAGNI (You Aren't Gonna Need It) principle. Create extension points based on actual needs rather than speculation. Document design decisions and tradeoffs.<br><br>
<br> [Top](#table-of-contents)

## Competencies in Data Structures and Algorithms
### Core Concepts
- **Understanding Data Structures**: Comprehend the fundamental data structures like arrays, linked lists, stacks, queues, trees, graphs, hash maps, and their respective operations.
- **Algorithm Design**: Familiarize yourself with sorting and searching algorithms, divide and conquer strategies, dynamic programming, greedy algorithms, recursion, and backtracking.
- **Efficiency Analysis**: Evaluate time and space complexity for various data structures and algorithms. Optimize solutions while ensuring correctness.
- **Scalability**: Understand scalability techniques such as caching, indexing, load balancing, and queues.

### Choosing Optimal Solutions
- **Toolbox Approach**: Build a mental toolbox of data structures suited for specific problems, e.g., quick access by key (hashmaps), sorting (trees), or dynamic resizing (lists).
- **Consider Edge Cases**: Be aware of potential pitfalls such as hash collisions in hashmaps or performance degradation in unbalanced trees.
- **Comparison and Justification**: When presenting a solution, justify your choice by comparing it with alternatives and highlight benefits and drawbacks.

### Analyzing Shortcomings and Tradeoffs
- **Identify Shortcomings**: Clarify limitations of the chosen data structure or algorithm upfront. Example: An array might be less suitable for frequent insertions than a linked list.
- **Discuss Tradeoffs**: Weigh pros and cons, e.g., recursive solutions are often elegant but can lead to stack overflow; dynamic programming might offer optimized solutions but at the expense of higher space complexity.
- **Alignment with Problem Patterns**: Align your solution with problem patterns, such as using DFS or BFS for graph problems, or dynamic programming for optimization challenges.

### Justifying Selection

- **Multiple Solutions**: When faced with a problem, it’s crucial to articulate the reasoning behind the chosen solution by comparing it with other potential approaches. For instance, if you choose a HashMap over a balanced binary search tree (BST) for key-value storage, discuss factors such as average-case retrieval time (O(1) for HashMap vs. O(log n) for BST) and tradeoffs like space complexity and potential for clustering in hash maps.

- **Data Structure Understanding**: Develop a deep understanding of how data structures function internally. Be prepared to explain the operations of data structures, such as why heap insertion is O(log n), how linked lists manage dynamic memory, or the methods of collision resolution in hash maps, like open addressing or chaining.

- **Consider Use Cases and Constraints**: Justify your selection based on the problem constraints. If a problem involves concurrent reads and writes, an array list may not be suitable due to its lack of thread safety, whereas a concurrent-friendly structure like a concurrent hashmap could be more appropriate.

### Demonstrating Runtime and Space Complexity

- **Complexity Analysis**: Clearly articulate the algorithm's time complexity (e.g., O(n log n) for mergesort) and space complexity. Even if you are not perfectly accurate in syntax, demonstrating an understanding of why certain complexities are associated with an algorithm or data structure is key.

- **Tradeoff Discussion**: Weigh time versus space tradeoffs, particularly in contexts where resources are constrained. Discuss scenarios where an algorithm might be faster but consumes more memory, and when it's pragmatic to compromise speed for reduced space usage, as in the case of in-place algorithms.

- **Real-world Constraints**: When the interviewer presents a problem, start by exploring all relevant data structures and algorithms. Consider theoretical constraints like memory limits, execution time requirements, and potential for parallel execution. Discuss which solutions are the best fit under these scenarios before proceeding.

- **Edge Cases Consideration**: Ensure you account for edge cases, such as handling empty datasets or extremely large inputs, which can affect runtime characteristics. Explain how your chosen algorithm or data structure handles these scenarios efficiently.
<br> [Top](#table-of-contents)
### Practice Topics

- **Binary Search Tree Operations**:
  - Understand inserting, deleting, and searching operations in-depth.
  - Practice implementing various traversal methods like in-order, pre-order, and post-order.
  - Recognize situations leading to unbalanced trees and solutions like AVL or Red-Black trees.

- **Common Algorithm Implementations**:
  - Write implementations from scratch for classic algorithms like quicksort and mergesort, noting how recursion and partitioning contribute to their time complexity.
  - Implement Dijkstra’s algorithm focusing on its use of priority queues for efficient pathfinding.
  - Explore Floyd-Warshall for all-pairs shortest paths and its O(n^3) complexity significance.

- **Memory Management**:
  - Investigate how different languages manage memory for data structures, especially languages with manual memory management like C++.
  - Understand garbage collection mechanisms and their implications for concurrent data structures.

- **Problem Solving on Platforms**:
  - Engage with platforms like LeetCode or HackerRank by solving problems that require nuanced decisions between data structures like heaps versus queues or linked lists versus dynamic arrays.

### Before the Interview

- Refresh key concepts of runtimes for basic operations (insert, delete, search) across different data structures.
- Familiarize yourself with the data structures provided by your programming language's standard library.
- Solve problems that feature algorithmic traversal patterns, such as DFS versus BFS.
- Contrast recursive solutions with iterative counterparts and explore their tradeoffs, notably in space consumption (stack space versus heap).

### During the Interview

- Engage with the interviewer to clarify problem requirements, constraints, and expectations.
- Propose several approaches initially and analyze their efficiencies, choosing one that balances speed and resource usage.
- Keep your code and thought process transparent, welcoming insights or corrections suggested by the interviewer.
- Demonstrate a command of both basic and advanced algorithmic approaches relevant to the problem at hand.

### Additional Resources

- **Books**: "Introduction to Algorithms" by Cormen, Leiserson, Rivest, and Stein; "The Algorithm Design Manual" by Steven Skiena.
- **Online Platforms**: Dive into LeetCode’s curated lists or job-specific interview challenges on CodeSignal.
- **Interview Archives**: Reviewing common problems and their solutions can give insights into frequently favored approaches and interviewer preferences.

### Common Pitfalls

- Overengineering simple solutions with unnecessarily complex data structures.
- Neglecting edge case analysis which could reveal performance bottlenecks.
- Misestimating algorithm complexity, especially in less familiar algorithms.

---

Note: Always approach each problem by considering multiple perspectives and be ready to discuss the tradeoffs for your choices.
<br> [Top](#table-of-contents)

## Problem Solving
### Core Concepts
- **Understanding Ambiguity**: Problems are often presented with incomplete or vague information. Your task is to navigate these uncertainties to pinpoint the core requirements.
- **Breaking Down Complex Problems**: Divide larger problems into manageable components and solve them incrementally.
- **Progressive Enhancement**: After your initial solution, refine and enhance it to meet evolving requirements or optimize performance.

### Uncovering Requirements and Evolution
- **Clarifying Questions**: Start by posing questions to the interviewer to ensure a full understanding of the problem. This sets the stage for comprehensive solution development.
- **Consider Future Changes**: Think ahead about how the problem might evolve or how additional requirements might be incorporated seamlessly into your existing solution.

### Implementing a First Pass
- **Initial Solution Development**: Focus on crafting an initial version that solves the problem, emphasizing correctness and clarity over optimization.
- **Structured Approach**: Write code that is well-organized and easy to follow, considering naming conventions and consistent styling practices.

### Enhancing and Evolving the Solution
- **Performance Analysis**: Once you have a working solution, identify potential bottlenecks and inefficient components to improve.
- **Iterative Improvement**: Enhance the solution by incorporating any additional feedback or evolving requirements shared during your discussion with the interviewer.

### Preparation Strategies
- **Practice Without an IDE**: Rehearse coding manually to strengthen your grasp on syntax and logical flow, as you'll often code on whiteboards or plain text editors during interviews.
- **Adaptability**: Develop agility in changing methods or ideas when new insights are presented. Practice solving problems with intentionally vague requirements.
- **Verbalize Thought Process**: Practice explaining your problem-solving steps out loud to improve clarity and communication with the interviewer.
- **Simplicity in Solution**: Resist unnecessary complexities. Implement solutions that are straightforward and directly address the given requirements.
<br> [Top](#table-of-contents)

### Demonstrating Your Competency
#### Correctly Solving the Problem
- **Edge Case Considerations**: Account for unusual inputs or conditions that may cause failures. Testing edge cases showcases thoroughness.
- **Validating Understanding**: Before you start coding, confirm that you have understood the problem statement fully, including constraints and scope.

#### Justifying Decisions
- **Evaluating Tradeoffs**: Discuss why one solution might be preferable over others, considering factors like time complexity, space complexity, and ease of implementation.
- **Iterative Solution**: It's better to have a working solution first and then improve upon it rather than aiming for perfect optimization initially.

#### Defining the Problem
- **Clarifying Requirements**: Ask targeted questions to clarify vague problem statements before jumping into code.
- **Testing Assumptions**: Use examples to validate your assumptions and discuss them with the interviewer to ensure alignment.

#### Additional Considerations
- **Descriptive Naming and Clarity**: Adhere to best practices in naming conventions and code organization for maintainability and readability.
- **Developer Effort and Team Dynamics**: Consider team skills and resources, ensuring solutions are accessible and implementable by diverse team members.

#### Minimal Hint Utilization
- **Test Case Development**: Prepare to propose and discuss test cases, both typical and edge ones, to validate your solution.
- **Directed Questioning**: Ask focused questions if you need hints. Communicating approaches you're considering can help the interviewer guide you constructively.

---

Note: Approach each problem by engaging both critically and creatively, validating your solutions through robust questioning and evidence-backed reasoning.
<br> [Top](#table-of-contents)

## Amazon Leadership Principles Overview

Amazon’s Leadership Principles guide business operations across all areas. Amazon Software Development Engineers utilize these principles daily, whether brainstorming new project ideas or deciding the best approach to problem-solving. A significant portion of interviews will focus on how you’ve demonstrated these Leadership Principles. Complete the steps below to reflect on your experiences with the Leadership Principles.

### Step 1: List Your Significant Professional Moments

List 10-15 significant professional experiences you’ve had. This includes goals achieved, risks taken, and instances of failure and growth. Don't worry about details now—focus on recalling the moments. Use your resume for memory triggers, prioritizing experiences from recent positions.

### Step 2: Recall the Specifics

Interviewers will dive deep into these examples, so it’s helpful to refresh your memory ahead of time. Use the STAR framework to recall details. Complete the table below for the first significant professional moment you listed in Step 1. Repeat for each moment.

#### Significant Professional Moment #1 STAR Framework

| STAR Component | Questions to Ask Yourself | Details |
|----------------|--------------------------|---------|
| Situation      | What was the context/background for the situation you were in? Where did it occur, when did it happen? What was the goal? |         |
| Task           | What was your role? What were you trying to achieve? Why was it important? What were the risks/consequences if nothing happened? |         |
| Action         | What did you personally own? How did you do it? How did you influence the outcome? Who else was involved? What was the most significant obstacle you faced? |         |
| Result         | How did you measure success for this project? What results did you achieve? (e.g., metrics) What trade-offs did you have to make to achieve this? What did you learn or would have done differently? |         |

### Step 3: Consider the Leadership Principles

With details fresh, identify which of the 16 Leadership Principles you demonstrated in each significant professional moment. Multiple principles may apply to each moment. All Leadership Principles are listed below for reference. Your experiences may not cover all 16—if needed, read through any unaddressed to see if they prompt additional memories for Step 1.

### Next Steps

Prepare to demonstrate to your interviewers how you’ve applied the Leadership Principles in your professional experiences. Bring a shortlist of significant moments to the interview and keep these tips in mind:
- **Answer the Interviewers’ Questions**: Don’t force examples that don’t address the interviewer’s questions.
- **Avoid Reading from a Script**: Use this guide to recall details accurately but avoid reading directly in the interview.
- **Remain Flexible**: Be ready for follow-up questions or requests for additional details.
- **Use a Range of Examples**: Showcase a variety of experiences.
- **Prioritize Recent Examples**: Use recent experiences for relevancy.

### Leadership Principles 

- **Customer Obsession**: Leaders start with the customer and work backwards. They work vigorously to earn and keep customer trust. Although leaders pay attention to competitors, they obsess over customers.
- **Ownership**: Leaders are owners. They think long term and don’t sacrifice long-term value for short-term results. They act on behalf of the entire company, beyond just their own team. They never say, “that’s not my job."
- **Invent and Simplify**: Leaders expect and require innovation and invention from their teams and always find ways to simplify. They are externally aware, look for new ideas from everywhere, and are not limited by “not invented here." As we do new things, we accept that we may be misunderstood for long periods of time.
- **Are Right, A Lot**: Leaders are right a lot. They have strong judgment and good instincts. They seek diverse perspectives and work to disconfirm their beliefs.
- **Learn and Be Curious**: Leaders are never done learning and always seek to improve themselves. They are curious about new possibilities and act to explore them.
- **Hire and Develop the Best**: Leaders raise the performance bar with every hire and promotion. They recognize exceptional talent, and willingly move them throughout the organization. Leaders develop leaders and take seriously their role in coaching others. We work on behalf of our people to invent mechanisms for development like Career Choice.
- **Insist on the Highest Standards**: Leaders have relentlessly high standards — many people may think these standards are unreasonably high. Leaders are continually raising the bar and drive their teams to deliver high quality products, services, and processes. Leaders ensure that defects do not get sent down the line and that problems are fixed so they stay fixed.
- **Think Big**: Thinking small is a self-fulfilling prophecy. Leaders create and communicate a bold direction that inspires results. They think differently and look around corners for ways to serve customers.
- **Bias for Action**: Speed matters in business. Many decisions and actions are reversible and do not need extensive study. We value calculated risk taking.
- **Frugality**: Accomplish more with less. Constraints breed resourcefulness, self-sufficiency, and invention. There are no extra points for growing headcount, budget size, or fixed expense.
- **Earn Trust**: Leaders listen attentively, speak candidly, and treat others respectfully. They are vocally self-critical, even when doing so is awkward or embarrassing. Leaders do not believe their or their team’s body odor smells of perfume. They benchmark themselves and their teams against the best.
- **Dive Deep**: Leaders operate at all levels, stay connected to the details, audit frequently, and are skeptical when metrics and anecdote differ. No task is beneath them.
- **Have Backbone; Disagree and Commit**: Leaders are obligated to respectfully challenge decisions when they disagree, even when doing so is uncomfortable or exhausting. Leaders have conviction and are tenacious. They do not compromise for the sake of social cohesion. Once a decision is determined, they commit wholly.
- **Deliver Results**: Leaders focus on the key inputs for their business and deliver them with the right quality and in a timely fashion. Despite setbacks, they rise to the occasion and never settle.
- **Strive to be Earth’s Best Employer**: Leaders work every day to create a safer, more productive, higher performing, more diverse, and more just work environment. They lead with empathy, have fun at work, and make it easy for others to have fun. Leaders ask themselves: Are my fellow employees growing? Are they empowered? Are they ready for what's next? Leaders have a vision for and commitment to their employees' personal success, whether that be at Amazon or elsewhere.
- **Success and Scale Bring Broad Responsibility**: We started in a garage, but we're not there anymore. We are big, we impact the world, and we are far from perfect. We must be humble and thoughtful about even the secondary effects of our actions. Our local communities, planet, and future generations need us to be better every day. We must begin each day with a determination to make better, do better, and be better for our customers, our employees, our partners, and the world at large. And we must end every day knowing we can do even more tomorrow. Leaders create more than they consume and always leave things better than how they found them.

[Top](#table-of-contents)

