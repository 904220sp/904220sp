- def run_quiz(questions):
    score = 0
    for question, options, correct_option in questions:
        print(question)
        for i, option in enumerate(options, start=1):
            print(f"{i}. {option}")

        user_answer = int(input("Enter the number corresponding to your answer: "))
        if user_answer == correct_option:
            print("Correct!\n")
            score += 1
        else:
            print(f"Wrong! The correct answer was {correct_option}: {options[correct_option-1]}\n")

    print(f"You scored {score}/{len(questions)}.")

# Example usage
quiz_questions = [
    ("What is the capital of France?", ["Paris", "Berlin", "Madrid"], 1),
    ("Which planet is known as the Red Planet?", ["Earth", "Mars", "Jupiter"], 2),
    ("What is the largest mammal?", ["Elephant", "Blue Whale", "Giraffe"], 2),
]

run_quiz(quiz_questions)

<!---
904220sp/904220sp is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
