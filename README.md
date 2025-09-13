# Model Fine Tuning and Bedrock Customization Example

This project demonstrates:
- Fine-tuning a Hugging Face transformer model for sentiment classification using custom data.
- Training and inference with AWS Bedrock custom models.

## Setup

1. **Prepare training data:**
   - Edit or extend `data/sample_training_data.jsonl` for your use case.

2. **Environment setup:**
   - Create venv if you prefer it that way


## Notes

- For Apple Silicon (M1/M2), PyTorch may default to MPS. The scripts force CPU to avoid device errors.
- You need AWS credentials configured for Bedrock API access.

## Files

- `fine_tune_hf.ipynb`: Jupyter Notebook for fine-tuning a Hugging Face transformer model.
- `aws_workflow.ipynb`: Jupyter Notebook for training and inference with AWS Bedrock custom models.
- `data/sample_training_data.jsonl`: Example training data.
