# Deep Flappy Bird
A Crazy Flappy Bird agent trained with Deep Reinforcement Learning 
> Support training on multiple platforms     
> e.g., Amazon EC2, Amazon SageMaker Notebook, Google Cloud Compute Engine, Google Colab

![game play](https://github.com/sizzle0121/Deep-FlappyBird/blob/main/GIF.gif)

[40 minutes version](https://drive.google.com/file/d/1EqPkHSgi2H_yW2NyRCQxY58HHk1lXriW/view?usp=sharing)

[Download the checkpoint of our best agent](https://drive.google.com/file/d/1q86V9zRVL8vzmWzD4SHgqSS_ucHQllI7/view?usp=sharing)

### Contributors
> Name: Fu-Lin Hsu     
> Name: James Hu    
> Name: Jonathan Choi

### Requirement
- Python 3.x
- Pygame
- Pytorch
- Numpy
- Opencv 3.x or later

### Before you start
1. Be sure you upload game assets in the directory order './assets/sprites/*.png'   
    + you can set the BASE_PATH as the prefix of assets/sprites/*.png, such as a mounted drive in Colab
    + Remember to end it with a slash '/'
2. Set up the directory you want to save checkpoints

### Environment

#### env.py
The Flappy Bird Game Environment    
To load resources (images) for the game, specify the __BASE_PATH__ parameter of __load()__  
Use __frame_step(input_actions)__ to interact with the game and get the next observation    
The game ends when the return value, __terminal__, of frame_step is True

#### env_utils.py
The utilities for establishing the environment

#### flappy_bird.py
The all-in-one training instance including game environment

#### flappy_bird_dueling.py
The all-in-one training instance using Dueling DQN
