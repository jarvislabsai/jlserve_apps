# Flux-Schnell

Fast text-to-image generation using Black Forest Labs' FLUX.1-schnell model.

## Description

FLUX.1-schnell is a fast distilled version of FLUX.1, optimized for 1-4 inference steps. Generates high-quality images from text prompts in seconds.

## Usage

```bash
jlserve dev app.py
```

## Example

```bash
curl -X POST http://localhost:8000/generate \
  -H "Content-Type: application/json" \
  -d '{
    "prompt": "A serene mountain landscape at sunset",
    "width": 512,
    "height": 512
  }'
```

## Requirements

- CUDA-capable GPU (recommended)
- ~18GB VRAM

## Model Info

- **Model**: black-forest-labs/FLUX.1-schnell
- **Type**: Text-to-Image Diffusion
- **Inference Steps**: 4 (optimized)
- **License**: Apache 2.0
