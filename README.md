# CTfeatureextraction

**Extracting features from Chest Tomography scans of patients to predict Covid 19 severity.**

The motivation behind this task was to find a way to integrate the effect of Chest Tomography scans in the prediction of severity of Covid 19.  
As seen in the second wave of Covid 19 during May 2021,CT scores played a major role in determination of severity,so giving an algorithm only the  
clinical factors seemed too not utilise it's potential to predict. Thus, CT scans were needed, and an efficient way to integrate them into our machine learning  
models.  
Pyradiomics seemed to serve the purpose of finding numerical features from the Chest scans although it needed image segments. Due to less quantity of radiologist  
annotated images, another algorithm was deployed to segment the major dataset of images using the pre annotated images. UNet was finalised to be used, as a efficient  
and powerful algorithm to annotate images. Once the segmented images were obtained they were used as an input along with the original images to extract numerical  
features out of them using PyRadiomics.


