# Image Generation with Diffusion Models

This notebook explores **text-to-image generation using diffusion models** from the Hugging Face ecosystem. Diffusion models generate images by starting from random noise and gradually denoising it while being guided by a text prompt.

---

## Workflow

1. Load a pre-trained diffusion pipeline from Hugging Face.
2. Provide a **text prompt** describing the desired image.
3. The model iteratively denoises random noise to produce an image aligned with the prompt.
4. Generated images are displayed within the notebook.

---

## Control Parameters

Several parameters were used to control image generation:

* **guidance_scale** – Controls how strongly the model follows the text prompt. Higher values make the output more aligned with the prompt.
* **num_inference_steps** – Number of denoising steps. More steps generally improve image quality but increase generation time.
* **seed / generator** – Fixes the random initialization so the same prompt produces the same image across runs.
* **negative_prompt** – Specifies features the model should avoid (e.g., blurry, low quality).

---

## Required Libraries

Install the following libraries before running the notebook:

```bash
pip install diffusers transformers accelerate torch safetensors matplotlib
```

These libraries provide the diffusion pipeline, deep learning backend, and visualization tools required for image generation.

---

## How to Run

1. Install the required dependencies.
2. Open the notebook in **Jupyter Notebook / VS Code**.
3. Run the cells sequentially.
4. Modify the text prompts to generate different images.

---


