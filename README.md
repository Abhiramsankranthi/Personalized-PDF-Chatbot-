Training Configuration
Your model was trained over 8 epochs using a dataset of 2,762 examples. The training was distributed across multiple devices, with each device processing an instantaneous batch size of 16.

To accommodate a larger effective batch size, gradient accumulation was used for 12 steps. This resulted in a total training batch size of 192 across all parallel processes. The entire training process involved 100 total optimization steps.

Model Parameters & Efficiency
The model has a total of 2.78 billion parameters. However, for efficient fine-tuning, Low-Rank Adaptation (LoRA) was employed. This technique significantly reduces the number of trainable parameters.

In this case, only 26,214,400 parameters were made trainable, which represents approximately 0.94% of the total parameters. This approach allows for efficient adaptation of the large model without needing to update all of its weights.
