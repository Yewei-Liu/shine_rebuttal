# LoRA

| num_sample \ num_epoch | 5            | 10          | 20          |
|------------------------|--------------|-------------|-------------|
| 3                      | 24.56(14.0)  | 27.78(28.1) | 35.05(56.1) |
| 5                      | 25.75(23.40) | 32.72(46.8) | 51.97(93.5) |
| 10                     | 32.81(46.8)  | 50.63(93.5)  | 58.50(187.0) |

# DoRA

| num_sample \ num_epoch | 5           | 10           | 20           |
|------------------------|-------------|--------------|--------------|
| 3                      | 24.48(17.0) | 27.90(34.0)  | 36.59(68.0)  |
| 5                      | 26.54(38.4) | 33.69(56.7)  | 48.67(113.3) |
| 10                     | 32.65(56.7) | 48.94(113.3) | 56.52(226.6) |


# IA3

| num_sample \ num_epoch | 5           | 10           | 20           |
|------------------------|-------------|--------------|--------------|
| 3                      | 24.60(12.7) | 26.31(25.38) | 29.06(50.7)  |
| 5                      | 25.26(21.2) | 28.2(42.3)   | 33.58(84.6)  |
| 10                     | 27.79(42.3) | 32.70(84.6)  | 38.25(169.2) |

Value in each grid means F1-Score(Time). Here F1-Score is tested on the test set of MS MARCO MQA, and the unit of time is seconds.

The left column shows the sample number. When num_sample = n, we generate n + 1 conversations for the same context in the same way. Among them, n conversations are used for fine-tuning, and 1 is used for testing. This corresponds to a very strong SFT setting. The top row shows the number of fine-tuning epochs.

SHINE achieves a score of 55.6(0.3) while requiring less time than fine-tuning a single sample for one epoch. 



