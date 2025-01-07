###To run the chatbot you have to:

You need to have Docker installed on your System.
(Use WSL2 on Windows to execute commands)

Run this command to train the model:

``docker run -v $(pwd):/app rasa/rasa:3.6.20-full train --domain domain.yml --data data --out models``

Afterwards run this command to start the rasa-shell:

``docker run -it -v $(pwd):/app rasa/rasa:3.6.20-full shell``
