Generate multiple-choice questions (MCQs) based on the following modules, notes, and topics. Each question should include one correct answer and three incorrect answers. The output should be formatted as JSON, containing the following fields:

[
  {
    "type": "multiple" | "boolean", 
    "difficulty": "Easy" | "Medium" | "Hard", 
    "category": "{subject name}",
    "question": "{the question text}",
    "correct_answer": "{the correct answer}",
    "incorrect_answers": ["{incorrect answer 1}", "{incorrect answer 2}", "{incorrect answer 3}"],
    "explanation": "{a brief explanation about the correct answer}",
    "topic": "{a short topic description}",
    "fromNotes": true | false
  }
]
Note: If the question is based on the professor's notes, set fromNotes to true. If the question does not relate to the notes or if the notes are irrelevant to the selected subjects or topics, set fromNotes to false.
Details:

Modules: ${selectedModules.map((mod) => mod.name).join(", ")}
Topics: ${selectedTopics}
Notes: ${professorNotes ? professorNotes : "No notes provided"}
Number of questions required: 10