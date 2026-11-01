# NLP Lab 10 — Introduction to Machine Translation

**Name:** Hadi Muneer Abu Allairat  
**Student ID:** 2230005761

Solution notebook: [`Lab10_Solution_Machine_Translation.ipynb`](Lab10_Solution_Machine_Translation.ipynb)

Neural machine translation with a Keras encoder–decoder LSTM. Tasks 1 and 2 are answered at the
end. The lab's own cells are kept unchanged, with analysis added underneath.

The main result is that the accuracy figure the lab prints is measuring padding, not translation.
The demo reports `Test Accuracy: 0.7143`, which is 5 of 7 padding positions on a single test
sentence; accuracy on real French words is 0.0000. Task 2 repeats the experiment on 20,000 real
sentence pairs and finds 0.69 reported against 0.08 on real words.

Task 2 links to a Kaggle dataset, which needs an account and an API token. I used an equivalent
public English–French corpus (OPUS-100 via Hugging Face), filtered to short pairs, and committed
the 20,000 pairs used as `dataset/en_fr_pairs_20k.csv`, so the notebook reproduces with no
credentials.

All cells are executed and their outputs saved. Every figure quoted in the written answers comes
from those outputs.
