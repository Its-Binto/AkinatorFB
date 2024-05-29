# AkinatorFB
The AkinatorFB application is designed to interactively predict football players based on a series of user-provided responses to questions about player attributes. The program employs a decision-making algorithm to narrow down the dataset iteratively, We are using the latest 2024 version of FC24 dataset. 
APPROACH AND LAYOUT
The AkinatorFC application is structured in a clear and modular manner, adhering to the best
practices in code layout and design, The code is organized into a class-based structure for
code organisation facilitates code readability, maintainability ,and reusability.
INITIALISATION:
LOAD THE DATASET:
The model starts by loading a dataset all_players.csv was downloaded from (Stefano Leone,
2023), which is initially being trimmed to essential columns needed for the guessing, Then
the trimmed dataset is saves as trimmed_dataset.csv, Then it is printed.
INITIALISE VARIABLES:
Track asked questions, Then the path taken during the game and a set of for players are
being declared to save.
USER INTERACTION LOOP:
The game is limited to ask 20 questions, asking for the users response to confirm or deny
specific attributes of the football player.
FILTERING DATASET:
Based on the user response (yes/no/probably(P)/probably-no(PN)t/I don’t know (idk)), the
dataset is filtered to narrow down the potential player matching the given criteria.’
PROBABLY AND PROBABLY-NOT LOGIC:
A ‘Probably (P)’ option is included to capture user uncertainty and a ‘Probably-not (PN)
option additional logic filtering player aged 25 and above to proceed cautiously.
PREDICTION HANDLING:
If only one player remains in the dataset, the model makes a prediction. If the prediction is
accurate, the game ends, and user feedback is requested. If not, the model learns from the
inaccurate prediction.
RANDOM QUESTION SELECTION:
In order to predict accurately and not to repeat the questions for making more user
interactive, Question are being asked randomly from the available columns and entries
which are taken from a sample of the dataset.
BEST GUESS:
The program comes with an additional feature called Best Guess, it is when the user
completes 20 question and the model wasn’t able to narrow down to one player. The model
makes the best guess based on the remaining dataset.
STRENGTHS AND WEAKNESSES
PROS:
INTERACTING AND ENGAGING : The game format makes it interactive and engaging for
users. Clear instructions and prompts contribute to a positive user experience.
RANDOMIZED QUESTION SELECTION: The use of randomization in selecting questions adds
an element of unpredictability, making each session potentially unique. This contributes to
user engagement and replay value.
ERROR HANDLING: The application includes error handling mechanisms to manage invalid
user inputs, ensuring the program can gracefully recover from unexpected scenarios.
CONS:
LIMITED DATASET EXPLORATION: The application only allows users to explore 20 questions
in the dataset, which may limit their ability to accurately predict answers to more
complicated queries. A more adaptive approach that adjusts the number of questions based
on the dataset size could be beneficial.
20 QUESTIONS MAX: The game has a 20 question maximum, which might not be the best
option in every situation.
ENHANCEMENTS
DYNAMIC QUESTION LIMIT: To ensure flexibility, introduce a dynamic question limit that is
dependent on the size of the dataset.
MACHINE LEARNING INTEGRATION: Incorporate machine learning algorithms for dynamic
learning from user feedback.
USER FEEDBACK ANALYSIS: Implement more characterised analysis of user feedback,
considering partial correctness and incorporating probabilistic predictions.
CONCLUSION
In conclusion, The implementation of features that improve adaptability, learning capacity
and user satisfaction, the proposed enhancements seek to elevate AkinatorFC24 model.
While this improvements comes with challenges, they open the door to creating a more
sophisticated and intelligent player prediction game.
REFERENCES
Stefano Leone. (2023, October). EA Sports FC 24 complete player dataset. Retrieved from
Kaggle: https://www.kaggle.com/datasets/stefanoleone992/ea-sports-fc-24-
complete-player-dataset
