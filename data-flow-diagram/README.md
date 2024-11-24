# Data Flow Diagram

A Data Flow Diagram (DFD) is a graphical representation of the flow of data through a system. It illustrates how data is processed by a system in terms of inputs and outputs.

## Levels of DFD

1. **Level 0 (Context Diagram)**: This is the highest level DFD which represents the entire system as a single process. It shows the system's interaction with external entities.

2. **Level 1**: This level breaks down the main process into sub-processes. It provides a more detailed view of the system.

3. **Level 2**: This level further decomposes the sub-processes into more detailed processes.

## Symbols Used in DFD

- **Process**: Represented by a circle or rounded rectangle, it shows the transformation of data.
- **Data Flow**: Represented by an arrow, it shows the direction of data movement.
- **Data Store**: Represented by an open-ended rectangle, it shows where data is stored.
- **External Entity**: Represented by a rectangle, it shows the sources or destinations of data outside the system.

## Example DFD for Airbnb Project

### Level 0 (Context Diagram)

```plaintext
+-------------------+       +-------------------+
|                   |       |                   |
|    User           |       |    Admin          |
|                   |       |                   |
+--------+----------+       +--------+----------+
         |                           |
         |                           |
         v                           v
+--------+---------------------------+--------+
|                                         |
|              Airbnb System              |
|                                         |
+-----------------------------------------+
```

### Level 1

```plaintext
+-------------------+       +-------------------+
|                   |       |                   |
|    User           |       |    Admin          |
|                   |       |                   |
+--------+----------+       +--------+----------+
         |                           |
         |                           |
         v                           v
+--------+---------------------------+--------+
|                                         |
|          1.0 Manage Listings            |
|                                         |
+--------+---------------------------+--------+
         |                           |
         v                           v
+--------+--------+          +--------+--------+
|                 |          |                 |
|  1.1 Add Listing|          |  1.2 View Listing|
|                 |          |                 |
+-----------------+          +-----------------+
```

### Level 2 (for Process 1.0 Manage Listings)

```plaintext
+-------------------+       +-------------------+
|                   |       |                   |
|    User           |       |    Admin          |
|                   |       |                   |
+--------+----------+       +--------+----------+
         |                           |
         |                           |
         v                           v
+--------+---------------------------+--------+
|                                         |
|          1.0 Manage Listings            |
|                                         |
+--------+---------------------------+--------+
         |                           |
         v                           v
+--------+--------+          +--------+--------+
|                 |          |                 |
|  1.1 Add Listing|          |  1.2 View Listing|
|                 |          |                 |
+--------+--------+          +--------+--------+
         |                           |
         v                           v
+--------+--------+          +--------+--------+
|                 |          |                 |
|  1.3 Edit Listing|         |  1.4 Delete Listing|
|                 |          |                 |
+-----------------+          +-----------------+
```

This is a basic representation of how data flows in an Airbnb project. Each process can be further decomposed to show more detailed data flow.
