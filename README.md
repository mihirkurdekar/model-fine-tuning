# Model Fine Tuning and Bedrock Customization Example

This project demonstrates:
- Fine-tuning a Hugging Face transformer model for sentiment classification using custom data.
- Training and inference with AWS Bedrock custom models.

## Setup

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Prepare training data:**
   - Edit or extend `data/sample_training_data.jsonl` for your use case.

## Fine-tune Hugging Face Model

Run:
```bash
python hf/fine_tune_hf.py
```
This script trains a sentiment classifier and tests it on a sample prompt.

## AWS Bedrock Custom Model

- Use `aws/bedrock_inference_example.py` to start a custom model training job and run inference.
- Update placeholders for S3 URIs, IAM role, and model IDs as needed.

## Requirements

See `requirements.txt` for Python package versions.

## Notes

- For Apple Silicon (M1/M2), PyTorch may default to MPS. The scripts force CPU to avoid device errors.
- You need AWS credentials configured for Bedrock API access.

## Folder Structure

- `hf/`: Hugging Face scripts.
- `aws/`: AWS Bedrock scripts.
- `data/`: Training and evaluation data.
- `requirements.txt`: Python dependencies.

## Files

- `hf/fine_tune_hf.py`: Hugging Face fine-tuning and test script.
- `data/sample_training_data.jsonl`: Example training data.
- `aws/bedrock_inference_example.py`: AWS Bedrock training/inference example.
- `requirements.txt`: Python dependencies.
