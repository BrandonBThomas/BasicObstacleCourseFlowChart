# BasicObstacleCourseFlowChart
Basic Obstacle Course FlowChart
'''mermaid
flowchart TD
    A[Obstacle Course] --> B(Balance Obstacle)
    B --> C[Use Hands] --> F
    B --> D[Hit Ground] --> F
    B --> E[Land On Finishing Platform] --> G
    F[Course Ends]
    G[Complete Obstacle] -->|Next Obstacle| H(Peg Board)
    H --> D
    H --> J[Drop Peg] --> F
    H --> K[Land On Finiashing Platform] --> L
    L[Complete Obstacle] -->|Next Obstacle| M(Warped Wall)
    M --> N[Miss] --> O
    O[Attempt 2] --> P
    P[Miss Again] --> Q
    Q[Attempt 3] --> R
    R[Miss] --> F
    M --> S
    O --> S
    Q --> S
    S[Clear Obstacle] --> T[Hit Buzzer]
    T --> U[Course Finish]
'''