# MONET CYCLEGAN PROJECT
This project tackles the unpaired image-to-image translation task of transforming ordinary landscape photos into Claude Monet–style paintings using a CycleGAN backbone. The base model employs dual generators and discriminators with cycle-consistency constraints so that a photo translated to Monet and back recovers its content, while adversarial training encourages the stylized output to mimic Monet’s color palette and brushwork.

The workflow begins with exploratory data analysis of the Monet and photo datasets, then builds TensorFlow input pipelines and trains the base CycleGAN while tracking generator and discriminator losses, per-epoch image snapshots, and best checkpoints. Next, we run targeted hyperparameter sweeps to select stable learning rates and optimizer settings, evaluate model quality with FID/MiFID metrics, and finally compare the base system against Least Squares, Hinge, and Wasserstein GAN variants to understand how different adversarial objectives impact style realism and content preservation.

---

**Note: I could not save the monet-gan.ipynb to GitHub after it had been fully ran because the file was too big. Please download the  pdf file Monet-GAN.pdf to see the entire report in its original format.**
