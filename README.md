# AWS-ViT

Implementing the vision transformer (ViT, https://arxiv.org/abs/2010.11929) on the cloud using AWS. Since AWS doesn't allow GPU's to new users we had to scale down the original ViT significantly. Using a c5.4xlarge instance (16 intel CPUs) we obtain a 75% classification accuracy on the CIFAR-10 dataset. Hyperparameters: 

Hyperparameter | value 
--- | --- 
Epochs | 20 
Batch size | 256
Optimiser | AdamW
Weight decay | 1e-4
Learning rate | 1e-3
Heads | 5
Patch size | 4
Layers | 6
Hidden MLP units | 128, 64 
MLP units | 512, 128
