Der bruges JSON frem for CSV, da dataenes kompleksitet er større, end hvad CSV egner sig til.
Et eksempel på et meget lille spørgsmålssæt:

    {
      subject: "arithmetic",
      questions: [
        {
          question: "Hvad er 1,5 + 2,5?",
          answers: [
            {
              answer: "4",
              correct: true
            },
            {
              answer: "12/3",
              correct: true
            },
            {
              answer: "5",
              correct: false
            },
            {
              answer: "7,5",
              correct: false
            }
          ],
          tags: [
            "matematik",
            "addition"
          ]
        },
        {
          question: "Hvad er 2^3?",
          answers: [
            {
              answer: "4",
              correct: false
            },
            {
              answer: "16",
              correct: false
            },
            {
              answer: "8",
              correct: true
            }
          ],
          tags: [
            "matematik",
            "exponentiering",
            "heltal"
          ]
        }
      ]
    }

Grammatikken er:

    QuestionSet = {
      subject: string,
      questions: [ Questions ]
    }

    Questions = Question[, Questions]

    Question = {
      question: string,
      answers: [ Answer, Answer[, Answer[, Answer]] ],
      tags: [ Tags ]
    }

    Answer = {
      answer: string,
      correct: boolean
    }

    Tags = string[, Tags]

