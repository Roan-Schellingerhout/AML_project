# AML_project

All the code used by team 25 for the AML food recognition project.

Each Jupyter notebook contains a model that is used to then.

The models used in the project are:
- Resnet 18
- Densenet 161*
- Densenet 121*
- BEiT (a modified version was used)
- Vit

All of the models have been used for the ensemble. The ensemble methods used are:
- A manual weighted ensemble
- A automatic ensemble
- A ensemble using a single model (BEiT)

To further the insight into the subject a background removal method was applied to the dataset. This was used as several papers showed promise in using pictures without backgrounds to further enhance the models understanding of the food presented. This is demonstrated in the two different datasets used (data & data2). The latter having no background.

However, it was soon found that it does not increase performance on most models. The only model to perform better was the densenet 161 model, densenet 121 performed about on par with or without the backgrounds. All other models performed worse that before the background removal.

*The densenet models share a notebook and the only changes that need to be made are to change out densenet 121 with densenet 161.
