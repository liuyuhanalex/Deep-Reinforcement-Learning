# Deep reinforcement learning
## Project Website
   [Let's play Pong!](https://liuyuhanalex.github.io/Deep-reinforcement-learning/)
## Team Members
- Hang Qi
- Jin Huang
- Yuhan Liu
- Yuxiang Bao

## Training the model
1. Download rlPong.py or rlPongTF.py(This version using tensorflow)
2. Install the require package using pip:
   - pickle: to store the model and arguements
   - tensorflow(if you want to use the tensorflow version)
   - gym: a toolkit for developing and comparing reinforcement learning algorithms
   - For windows users, you can install gym[atari] without cmake using this way:
     - pip install --no-index -f https://github.com/Kojoley/atari-py/releases atari_py
     - pip install git+https://github.com/Kojoley/atari-py.git
3. Using your parameters to train the model
   - python rlPong.py(rlPongTF.py) a b c d e
     - a: Number of hidden layer neurons
     - b: Batch size to update
     - c: Learning rate
     - d: Discount factor for reward
     - e: Decay factor for RMSProp leaky sum of grad^2
4. You can stop whenever you want, and if you want to resume last training:
   - python rlPong.py(rlPongTF.py) resume
