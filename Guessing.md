```mermaid
flowchart TD
A([Start]) --> B[Generate Random Number]
B --> C[Ask for User Guess]
C --> D {Is Input Valid?}
D --> |Yes| E[Check Guess]
D --> |No| F[Display "Invalid Input"]
F --> C
E --> |Correct| G[Display "Win!"]
E --> |Too High| H[Display "Too High"]
E --> |Too Low| I[Display "Too Low"]
H --> C
I --> C
G --> J([End])
```
