# smile_detector
Creating Smile / Frown Classifier App

Before starting this project I thought it would be a simple exercise to practice skills learned during the 2nd and 3rd lessons of FastAI. Overall this is a huge success - I have learned and practiced a lot, and not only the machine learning / AI coding but the behid-the-hood, real data science model experience.

Initially, I wanted to create an emotion classifier: happy, sad, neutral. However, I ran into several problems:
1. Happy, sad and neutral are too ambiguous for computer. What does it meean to be happy? Is it closing your eyes and tilting your head slightly to the side, or is it laughing? What is sad? And even though I was getting relatively OK error rate on the validation sets, once I started uploading my own pictures it started failing pretty bad. After many iterations I realized that the task of emotion recognition is too ambitious for the beginner friendly first project and switched to the smile / frown recognition - which probably is the right approach for building more complex emotion identification - start by identifying individual features first.
2. I ran into the problem of very poor training data sourced from Bing. There were plenty of smiles / happy in sad / frown pulls and vice versa.
3. Hyperparameter tuning is crucial and highly dependent on the task at hand. For this task the key parameter was the min_scale when creaing a DataBlock for training.
