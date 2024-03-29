# Attention-Augmented CNN For Text Classification
This is my implementaion of single-layer [attention-augmented CNN](https://arxiv.org/abs/1904.09925) for Text Classification (Sentiment Analysis) of movie reviews on the [MR](http://www.cs.cornell.edu/people/pabo/movie-review-data/) dataset. The model is implemented as a `Seq2VecEncoder`in [AllenNLP](https://github.com/allenai/allennlp).

## Intstructions:

* Install Allennlp and the requirments with `pip install -r requirments.txt`
* Configure the `experiments/review_classifier.json` for hyperparameters. Just make sure to have `padding_length` in the dataset_reader configuration to be the same as `sequence_length` in the sentence encoder configuration.
* Train the model with: 

` allennlp train experiments/review_classifier.json -s /out_dir --include-package my_library -f`

