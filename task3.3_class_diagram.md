<<<<<<< HEAD
=======
@startuml

class Child {
    - id: int    
    - name: string
    - age: int
    - progress: float
    + completeTask(task: Task): float -- updates progress
    + determineTaskSet(progress: float): List<Task>
}

class Task {
    - id: int
    - instruction: string
    - pictures: Map<string, string>
    - feedback: string
    + checkAnswer(answer: string): boolean
    + generateFeedback(isCorrect: boolean): void
}

class Parent {
    - id: int
    - name: string
    - password: string
     - children: List<Child>
    + viewChildProgress(child: Child): string
    + setAppUsageTime(child: Child, time: int)
}

class Administrator {
    - id: int
    - username: string
    - password: string
    + createTask(task: Task): void
    + editTask(task: Task): void
    + deleteTask(task: Task): void
    + manageUser(child: Child, parent: Parent): void
}

Child "1" --> "*" Task : completes
Parent "1" --> "*" Child : has
Administrator "1" --> "*" Parent : manages
Administrator "1" --> "*" Child: manages
Administrator "1" --> "*" Task : creates

@enduml
>>>>>>> 7ab480dc8fc925c7b872ea39e9ecf149e5261ba4
