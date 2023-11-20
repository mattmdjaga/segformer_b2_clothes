# Clothing semantic segmentation

This repo provides the code that I used to train the model [mattmdjaga/segformer_b2_clothes](https://huggingface.co/mattmdjaga/segformer_b2_clothes) on hugging face using the [mattmdjaga/human_parsing_dataset](https://huggingface.co/datasets/mattmdjaga/human_parsing_dataset) dataset which is a copy of the [ATR dataset](https://github.com/lemondan/HumanParsing-Dataset) for clothes segmentation but can also be used for human segmentation.

Requirements:
- PyTorch
- Transformers
- Evaluate
- Albumentations
- Wandb
- Datasets

## Training

For training I prefer using pure PyTorch over the Hugging Face Trainer API. Mainly because I like to have more control over the training loop and I like to use the [Wandb](https://wandb.ai/) library for logging.
