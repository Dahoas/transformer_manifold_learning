# transformer_manifold_learning

## Experiment Design

- examine impact of model size
- position in context
- source of data (reddit vs. arxiv)
- task
- change across each layer?

training from scratch vs. using pre-trained models?

Perhaps I should keep the ratio of kth neareast neighbor to number of samples constant?
- larger samples causes larger int. dim
- larger k (NN) causes smaller int. dim
    - this counteracts using more samples
    - why?
    - roughly K $\approx$ n to keep things stable
        - with this things do appear more stable than in tom goldstein paper

Tom goldstein paper uses $\alpha$ many points as anchors and averages local int. dim estimatse using this

Dim. of tinyStories seems to be somewhere around 9

Datasets:
- roneneldan/TinyStories

Models:
- gpt2
- gpt2-large

"So we use the activations from the last token in each
sequence to measure the ID, though the ID does not vary significantly across token positions"