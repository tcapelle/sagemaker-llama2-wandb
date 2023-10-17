# Finetuning CodeLlama on the Weights & Biases API

In this repo you have the relevant code to train a CodeLLama model on instruction dataset gathered by the [wandbot](github.com/wandb/wandbot).
- It uses the Huggignface Integration with Sagemaker
- Formats the dataset accordingly
- Evaluates the model in freshly gathered data

> More info on the HF tools used: [transformers](https://huggingface.co/docs/transformers/index), [datasets](https://huggingface.co/docs/datasets/index).

# Training
* [Data preparation with W&B](./training/01_data_prep.ipynb)
* [Fine-tune CodeLLaMA on Amazon SageMaker](./training/02_training_codellama.ipynb) 

## Requirements

Before we can start make sure you have met the following requirements

* AWS Account with quota
* [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed
* AWS IAM user [configured in CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) with permission to create and manage ec2 instances