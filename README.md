<h3>Simple image classifier for histopathology samples (colon)</h3>
<h3>Model generation is in preprocessing.ipynb</h3>
<h3>To simply run the model on your data, run deployment.ipynb</h3>
<h3>Sample data are in the folders (online/colon_aca - malignant and online/colon_n - healthy)</h3>


This is a quick and simple FastAI (https://docs.fast.ai/) implementation of an image classifier for histopathology images of colon to determine if they're of healthy or cancerous tissue.<br><br>
It uses a pretrained model (Squeezenet1_1) and the specific dataset used for further training is of 350 healthy and 350 cancerous images - randomly sampled from a database of about 25000 images. The rationale for using Squeezenet as the architecture was to keep the size of the trained model to where it could be included in a free GitHub repository. That said, it performs very well on its own merits and holds up against ResNet-34 for this particular task.<br><br>
The dataset was taken from Kaggle: kaggle.com/andrewmvd/lung-and-colon-cancer-histopathological-images . <br> <br>
Borkowski AA, Bui MM, Thomas LB, Wilson CP, DeLand LA, Mastorides SM. Lung and Colon Cancer Histopathological Image Dataset (LC25000). arXiv:1912.12142v1 [eess.IV], 2019. <br><br>
It's amazing how well the model does with very little training - 99.3% accuracy on testing data! - though, admittedly, the database used does have big differences between healthy and cancerous histopathology images. It would be great to try out the model on a more challenging dataset and go from there. <br><br>
