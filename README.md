# Medical Chatbot using DeepSeek-R1

This project builds a clinical reasoning medical chatbot by fine-tuning the [DeepSeek-R1 Distill Llama 8B](https://huggingface.co/dee/DeepSeek-R1-Distill-Llama-8B) language model. The workflow is provided in a Google Colab notebook that covers the full pipeline from model loading, inference, parameter-efficient fine-tuning, to evaluation.

## Features

- **Medical QA Chatbot**: Answers complex clinical questions with step-by-step, chain-of-thought explanations.
- **Efficient Training**: Uses [Unsloth](https://github.com/unslothai/unsloth) for fast LLM operations and [LoRA](https://arxiv.org/abs/2106.09685) for parameter-efficient finetuning.
- **Domain-specific Dataset**: Fine-tunes on the [FreedomIntelligence/medical-o1-reasoning-SFT](https://huggingface.co/datasets/FreedomIntelligence/medical-o1-reasoning-SFT) medical reasoning dataset.
- **Experiment Tracking**: Integrates with [Weights & Biases](https://wandb.ai/) for training monitoring.
- **Colab-Ready**: Designed for easy reproducibility and GPU acceleration in Google Colab.

## Usage

1. **Setup**: Upload and open the notebook in Google Colab.
2. **Configure Tokens**: Provide your Hugging Face and Weights & Biases tokens via Colab's `userdata`.
3. **Run Cells**: Execute each cell sequentially to install dependencies, load the model, run inference, and (optionally) fine-tune the model.
4. **Test**: Try medical questions and review the chatbot’s detailed, step-by-step answers.

## Project Structure

- **Model Loading**: Loads DeepSeek-R1 8B in 4-bit for resource efficiency.
- **Prompt Engineering**: Uses clinical expert persona and stepwise reasoning in responses.
- **Fine-tuning**: Parameter-efficient LoRA adaptation on medical chain-of-thought data.
- **Evaluation**: Test cells for post-training medical QA.

## Requirements

- Google Colab (with GPU)
- Hugging Face account and token
- Weights & Biases account and API key (optional, for experiment tracking)

## License

This project is for educational and research purposes only. Not for clinical or diagnostic use.

---
