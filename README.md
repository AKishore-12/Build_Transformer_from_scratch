# Build Transformer from scratch

A minimal, educational implementation of a GPT-style Transformer language model using PyTorch. This project demonstrates the core ideas behind modern large language models, including tokenization, self-attention, multi-head attention, and autoregressive text generation.

## Features

- Implements a character-level Transformer (GPT) from scratch in a single Python file.
- Trains on any text file (default: `input.txt`).
- Generates new text samples after training.
- Simple, readable code with no external dependencies beyond PyTorch and NumPy.

## Project Structure

- `gpt.py` — Main script containing the model, training loop, and text generation logic.
- `input.txt` — Training data (provide your own large text file for best results).
- `requirements.txt` — List of required Python packages.

## Requirements

- Python 3.7+
- PyTorch
- NumPy

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage

1. **Prepare your data:**  
   Place your training text in `input.txt`. The script will use this file to build its vocabulary and train the model.

2. **Train the model:**  
   Run the main script:

   ```bash
   python gpt.py
   ```

   - The script will print training and validation loss periodically.
   - After training, it will generate a sample of text and print it to the console.

3. **Customizing hyperparameters:**  
   You can adjust model and training parameters (like `batch_size`, `block_size`, `n_embd`, `n_head`, `n_layer`, etc.) at the top of `gpt.py`.

## Output

- After training, the script generates a sample of text using the trained model and prints it to the terminal.
- You can modify the script to save generated text to a file if desired.

## Notes

- This implementation is for educational purposes and is not optimized for large-scale training or deployment.
- For best results, use a large and diverse `input.txt` file.
