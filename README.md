# Autoregressive Visual Encoder Visualization

An interactive visualization demonstrating how autoregressive models generate images token by token, followed by a decoder smoothing phase.

## Features

- **Token-by-Token Generation**: See how the model predicts 16×16 pixel patches sequentially
- **Decoder Smoothing**: Watch the blocky tokens transform into a smooth final image
- **Interactive Speed Control**: Adjust generation speed to better understand the process
- **AI Realist Color Palette**: Human-centered design with coral, deep brown, soft cream, and muted purple

## Usage

1. Start the server:
   ```bash
   python3 -m http.server 8000
   ```

2. Open http://localhost:8000 in your browser

3. The demo automatically loads with a default image and starts generating

4. Upload your own images to see the autoregressive generation process on different content

## How It Works

1. **Autoregressive Generation**: The model generates one 16×16 token at a time, predicting each patch based on previous ones
2. **Discrete Tokens**: Each token is represented as a blocky, quantized patch
3. **Decoder Phase**: After all tokens are generated, a decoder gradually smooths them into the final high-quality image

This visualization helps understand the two-stage process used in modern autoregressive visual models.
