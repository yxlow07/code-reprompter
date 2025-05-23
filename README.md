## Code Re-prompter and Evaluator
This is a simple AI-based re-prompter and evaluator for solving complex problems that require multiple iterations to get right. The AI evaluating the problem can be interchanged with any other AI model, such as OpenAI's GPT-4.1 or Claude AI.

## Brief Overview
The code takes in a problem statement, generates code to solve the problem, and then evaluates the code to determine if it meets the requirements. If the code does not meet the requirements, it generates a new prompt to improve the code. This process continues until the code meets the requirements or a maximum number of iterations is reached. This is an extremely simplified version of Google's Alpha Evolve, which includes a component to improve the prompt based on the evaluation of the code. 

## Usage Guidelines
1. All of the code is in main.ipynb. Ensure you have jupyter installed to run the notebook.
2. Paste the problem statement into `problem.txt`, expected output into `expected.txt`, and inputs into `input.txt`.
3. Run ALL the cells in the notebook, this includes installing necessary libraries and loading the models.
4. The code will generate a solution to the problem, evaluate it, and if necessary, improve the code.
5. All system prompts are stored in `prompt-{function}.txt` files. You can modify these prompts to change the behavior of the AI.
6. The code is designed to be modular, so you can easily swap out the AI model used for evaluation or code generation. Simply modify the `generate` function to use a different model.
7. Convert the code to other languages if necessary.

## Further Improvements
1. Add more sophisticated evaluation metrics to determine if the code meets the requirements.
2. Implement a more advanced prompt improvement strategy based on the evaluation results.