const prompt = `
      Generate multiple-choice questions (MCQs) based on the following modules and topics. 
      Each question should have one correct answer and three incorrect answers. 
      Provide the output in JSON format.
      The JSON must contain 
      [
      type: "multiple or boolean",{if it is boolean then the options must be true or false or else 4 options out of which 1 is corrcet and 3 are incorrect}
      difficulty: "Easy,"Medium" or "Hard", 
      category: {add subject name here},
      question,
      correct_answer,
      incorrect_answers: [{array of other 3 incorrect answers}
      topic: {question related to which topic, if it is too long then make it short}
      ]

      Modules: ${selectedModules.map((mod) => mod.name).join(", ")}
      Topics: ${selectedTopics}
      Number of questions required: 20
    `;