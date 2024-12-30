@startuml

class Child {
    - id: int    
- name: string
    - age: int
    - progress: Map<Task, string>
    + completeTask(task: Task): void
}

class Task {
    - id: int
    - instruction: string
    - pictures: Map<string, string>    - feedback: string
    + checkAnswer(answer: string): boolean
    + generateFeedback(isCorrect: boolean): void
}

Child "1" --> "*" Task : completes

@enduml
