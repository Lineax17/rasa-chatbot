You need to have Docker installed on your System.

Run this command to train the model:

'''
docker run -v $(pwd):/app rasa/rasa:3.6.20-full train --domain domain.yml --data data --out models
'''

Afterwards run this command to start the rasa-shell:

'''
docker run -it -v $(pwd):/app rasa/rasa:3.6.20-full shell
'''
