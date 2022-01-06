# sartorius-cell-submission
<pre>
Step-wise procedure used to obtain file for Kaggle Submission
File links after execution of each of the sections from jupyter notebook attached:  
1. Training with all of LiveCell data using Cascade Mask RCNN: 
    input - markunys livecell data; attached annotation files; 
    output - <a href="https://drive.google.com/file/d/1-o3JVPLWx070rMrOxNHM4V-kHIANm2vG/view?usp=sharing" title="title">model_best.pth</a> 
2. Transfer Learning using Sartorius Dataset: 
    input - <a href="https://drive.google.com/file/d/1dPbOf9e480hx0sxVFGyo93B40sJMQUDl/view?usp=sharing" title="title">coco_cell_valid_fold4.json</a>; <a href="https://drive.google.com/file/d/1qvjruUgvlgfUY_K0YS_fiPlu3f6FLK-a/view?usp=sharing" title="title">coco_cell_train_fold4.json</a>; Sartorius Dataset
    output - <a href="https://drive.google.com/file/d/1CVWavXTMyjdT8IoiAW4AuDoV1qiO8VaJ/view?usp=sharing" title="title">model_best.pth</a>
2. Inference on all Semi-Supervised data to create .json pseudo_labels file; 
    input - jsons and model_best.pth from previous step; Semi Supervised Learning Dataset
    output - <a href="https://drive.google.com/file/d/1dOgM3O0YhNNoRvbedwV9DEMbxX_U-4bu/view?usp=sharing" title="title">pseudo_labels_f4.json</a> 
3. Training with pseudo labels and train dataset
    input - jsons from previvious step with newly creating pseudo json; Sartorius Dataset
    output -  <a href="https://drive.google.com/file/d/1dOgM3O0YhNNoRvbedwV9DEMbxX_U-4bu/view?usp=sharing)" title="title">model_best.pth</a>  (final file used during inference on Kaggle Submission) 

</pre>
