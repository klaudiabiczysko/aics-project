# Notes
- Used settings and hyperparameters

## Bert model 
Scores for the pre-trained BertClassifier(), trained on 5, 10 and 20 epochs. 
- Tokenizer: BertTokenizer('bert-base-cased')
- Hyperparameters: LR=1e-6.

| Epochs | Accuracy |
| ------ | ------ |
| 5 | 58.3% |
| 10 | 56.8% |
| 20 | 56.5% |

- Tested also other LR, such as: [1e-7, 0.001, 0.01, 0.1, 0.2, 0.3]
- Tested multilingual BertTokenizer.
- The scores were much lower than 56%, hence not reported. 
