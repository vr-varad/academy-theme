---
title: '{{ replace .File.ContentBaseName `-` ` ` | title }}'
pass_percentage: 70 # Minimum percentage required to pass the quiz
time_limit: 15 # Duration of the quiz in minutes
difficulty: "beginner" # Difficulty level of the quiz 
category: "Programming Languages" # Category of the quiz
tags: ["golang", "basics", "syntax", "fundamentals"] # Tags for the quiz, useful for search and categorization
type: "quiz" # Type of the content, in this case, a quiz ( required for the quiz to be recognized by the system )

questions:
  # Multiple Choice Question (Single Answer)
  - id: "q1"
    text: "What keyword is used to define a function in Go?"
    type: "mcq"
    marks: 2
    explanation: "The 'func' keyword is used to declare functions in Go, similar to how 'function' is used in JavaScript."
    options:
      - id: "a"
        text: "function"
        is_correct: false
      - id: "b"
        text: "def"
        is_correct: false
      - id: "c"
        text: "func"
        is_correct: true
      - id: "d"
        text: "fn"
        is_correct: false

  # Short Answer Question
  - id: "q2"
    text: "Go is a statically typed language. (true/false)"
    type: "short_answer"
    marks: 2
    correct_answer: "true"
    case_sensitive: false
    explanation: "Go is indeed a statically typed language, meaning variable types are determined at compile time."

  # Short Answer Question (Numeric)
  - id: "q3"
    text: "What is the zero value of an uninitialized int in Go?"
    type: "short_answer"
    marks: 2
    correct_answer: "0"
    explanation: "In Go, the zero value for numeric types like int is 0."

  # Multiple Choice Question (Multiple Answers)
  - id: "q4"
    text: "What are the purposes of the 'defer' keyword in Go? (Select all that apply)"
    type: "mcq"
    multiple_answers: true
    marks: 2
    explanation: "The defer keyword is commonly used to delay function execution until the surrounding function returns, often used for cleanup tasks like closing files."
    options:
      - id: "a"
        text: "To delay the execution of a function until the surrounding function returns"
        is_correct: true
      - id: "b"
        text: "To define a constant value"
        is_correct: false
      - id: "c"
        text: "To close resources like files or network connections"
        is_correct: true
      - id: "d"
        text: "To handle errors in a function"
        is_correct: false
---

This quiz will test your understanding of basic Go language features including syntax, type system, and key language constructs.
