# Pretrained Models and Image Transforms

This project uses pretrained models from the [timm](https://github.com/huggingface/pytorch-image-models) library.  
All models are used in evaluation mode.

---

## Model URLs

| Model | Source |
|-------|---------|
| BEiT Base Patch16 224 | https://huggingface.co/timm/beit_base_patch16_224 |
| ConvNeXt Tiny | https://huggingface.co/timm/convnext_tiny |
| ResNet-101 | https://huggingface.co/timm/resnet101 |
| ViT Base Patch16 224 | https://huggingface.co/timm/vit_base_patch16_224 |

---

## Hyperparameters

| Parameter | Value |
|------------|--------|
| Input size | 224 × 224 |
| Learning rate | N/A (pretrained only) |
| # Epochs | 0 (inference only) |
| NN Algorithm | Pretrained via `timm.create_model()` |


## Datasets Used in HW3

| Dataset | URL | Purpose |
|----------|-----|----------|
| **ImageNet-1K** | https://huggingface.co/datasets/imagenet-1k | Validation / Testing |
| **ImageNet Classes File** | https://raw.githubusercontent.com/pytorch/hub/master/imagenet_classes.txt | Class label names |