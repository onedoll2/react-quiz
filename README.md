# React Simple Quiz

a react component to quiz for learning

## Demo

![react-simple-quiz](https://user-images.githubusercontent.com/82763682/143409938-c0ca207e-deea-4b59-abd2-d595a4b1f9ad.gif)

## Installation

```
npm install --save react-simple-quiz
```

## Usage

```
import { ReactQuiz } from "react-simple-quiz";

//...

function App() {
  const quiz = [
    {
      id : 1,
      question: "Which country is not in Asia? ",
      answers : [
        {text : "Korea", isCorrect : false},
        {text : "Japan", isCorrect : false},
        {text : "China", isCorrect : false},
        {text : "USA", isCorrect : true},
      ]
    },
    {
      id : 2,
      question: " Which country is not in Africa?",
      answers : [
        {text : "Morocco", isCorrect : false},
        {text : "Jamaica", isCorrect : true},
        {text : "Libya", isCorrect : false},
        {text : "Congo", isCorrect : false},
      ]
    },
    {
      id : 3,
      question: "  Which country is not in Europe?",
      answers : [
        {text : "France", isCorrect : false},
        {text : "Germany", isCorrect : false},
        {text : "Argentina", isCorrect : true},
        {text : "England", isCorrect : false},
      ]
    },
  ]

  return <ReactQuiz quiz={quiz}/>
}
```

## Props

### 1. id

- required
- number

This props means the sequence number of the quiz.

### 2.question

- required
- srting

This is the contents that will be used for question.

### 3. answers

- required
- any

This prop sets the answers to the quiz questions.

### 4. text

- required
- any

This is the contents that will be used for the answers of the quiz.

### 5. isCorrect

- required
- boolean

Give true for the correct answer and false for the incorrect answer.
