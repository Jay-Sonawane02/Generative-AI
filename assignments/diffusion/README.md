# Image Generation with Diffusion Models

This notebook explores **text-to-image generation using diffusion models** from the Hugging Face ecosystem. A diffusion model generates images by starting from random noise and gradually denoising it while being guided by a text prompt.

---

## Workflow

1. Load a pre-trained diffusion pipeline from Hugging Face.
2. Provide a **text prompt** describing the desired image.
3. The model iteratively denoises random noise to produce an image aligned with the prompt.
4. Generated images are displayed within the notebook.

---

## Control Parameters

Several parameters were used to control image generation:

* **guidance_scale** – Controls how strongly the model follows the text prompt. Higher values make the image more aligned with the prompt.
* **num_inference_steps** – Number of denoising steps. More steps generally produce higher quality images but increase generation time.
* **seed / generator** – Fixes the random initialization so the same prompt produces the same image across runs.
* **negative_prompt** – Specifies features to avoid in the generated image (e.g., blurry or low quality).

---

## Technologies Used

* Python
* Hugging Face `diffusers`
* PyTorch
* Matplotlib

---
