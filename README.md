# Emotional-Support-Conversation
Data and codes for the ACL 2021 paper: [**Towards Emotional Support Dialog Systems**](https://arxiv.org/abs/2106.01144)

If you have any problem or suggestion, feel free to contact me: chujiezhengchn@gmail.com

## Data

We have collected **more** conversations with more topics. ESConv now contians 1,410 conversations with 10 topic problems.

You can run `python process.py` to process the data, and the processed results will be fed into the latter experiments.

## Model Implementation

The model implementation is integrated by  [@chujiezheng](https://github.com/chujiezheng) in the repo [chujiezheng/UniModel (github.com)](https://github.com/chujiezheng/UniModel).

## Bug

If you reproduce our experiments, you may find that the calculated ppl is a bit higher than the results reported in our paper. That is because we mistook the average of ppl of utterances as the final result, which should instead be calculated by averaging the tokens in all the test corpus.

