# Reconchess-CS748

# Chess Game Replay and Analysis

This repository includes scripts for replaying chess games, evaluating move scores, and analyzing performance against different bots. Additionally, Jupyter Notebooks are provided for calculating win percentages and training the weights of the lc0 network.

## Usage

1. **Activate Virtual Environment:**

    ```bash
    conda activate <path-to-your-virtualenv>
    ```

2. **Replace Files:**

    Copy and replace the following files in your project with their buffer counterparts:
   
    - `fianchetto_bot.py`
    - `strangefish_bot.py`
    - `multiprocessing_strategies.py`

3. **Run Scripts:**

    - To generate a replay buffer:

        ```bash
        python scripts/buffer.py <Path to the game you want to replay>
        ```

        For example:

        ```bash
        python scripts/buffer.py /home/puranjay/Fianchetto_IIT_Bombay/Fianchetto_fast/655504.json
        ```

    - To replay a game and display move scores and top board probabilities:

        ```bash
        python scripts/buffer_replay.py <Path to game you want to replay>
        ```

        For example:

        ```bash
        python scripts/buffer_replay.py /home/puranjay/Fianchetto_IIT_Bombay/Fianchetto_fast/655504.json
        ```

## Jupyter Notebooks

- **Winrate_Fianchetto.ipynb:**
  Use this notebook to find the win percentage against various bots on the RBC server.

- **NewOpponentModel.ipynb:**
  This notebook was used to train the weights of the lc0 network.

