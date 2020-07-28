# Removing Unfair Bias in Machine Learning

## Details

AI can embed human and societal bias and be then deployed at scale. Many algorithms are now being reexamined due to illegal bias. So how do you remove bias & discrimination in the machine learning pipeline? In this workshop you will learn the debiasing techniques that can be implemented by using the open source toolkit AI Fairness 360.

AI Fairness 360 (AIF360) is an extensible, open source toolkit for measuring, understanding, and removing AI bias. It contains the most widely used bias metrics, bias mitigation algorithms, and metric explainers from the top AI fairness researchers across industry & academia.

You will learn:
how to measure bias in your data sets & models
how to apply the fairness algorithms to reduce bias
how to apply a practical use case of bias measurement & mitigation

## Getting Started with Jupyter Notebooks

Jupyter notebooks are an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text.

In this workshop we will use IBM Watson Studio to run a notebook. For this you will need an IBM Cloud account. The following steps will show you how sign up and get started. When you have the notebook up and running we will go through the notebook.

## IBM Cloud

- [Sign up](http://ibm.biz/ai_fair_workshop) for an IBM Cloud account

- When you are signed up click `Create Resource` at the top of the Resources page. You can find the resources under the hamburger menu at the top left:

![](https://github.com/IBMDeveloperUK/python-geopandas-workshop/blob/master/images/Create_resource.png)

- Search for Watson Studio and click on the tile:

![](https://github.com/IBMDeveloperUK/jupyter-notebooks-101/blob/master/images/studio.png)

- Select the Lite plan and click `Create`.
- Go back to the Resources list and click on your Watson Studio service and then click `Get Started`.

![](https://github.com/IBMDeveloperUK/jupyter-notebooks-101/blob/master/images/launch.png)

## IBM Watson Studio

### 1. Create a new Project

- You should now be in Watson Studio.
- Create a new project by clicking on `Get Started` and `New Project`, or `Create Project`
- Give your Project a name.
- Select an Object Storage from the drop-down menu or create a new one for free. This is used to store the notebooks and data. **Do not forget to click refresh when returning to the Project page.**
- click `Create`.  

### 2. Load and run a notebook

- Add a new notebook. Click `Add to project` and choose `Notebook`:

![](https://github.com/IBMDeveloperUK/python-geopandas-workshop/blob/master/images/notebook.png)

- Choose new notebook `From URL`. Give your notebook a name and copy the URL `https://github.com/IBMDeveloperUK/geopandas-workshop/blob/master/notebooks/geopandas-workshop.ipynb`
- Select the custom runtime enviroment that you created and click `Create Notebook`.
- The notebook will load.

You are now ready to follow along with the workshop in the notebook!

## Anaconda local install

`> conda create --name aif360 python=3.7`

`> conda activate aif360`

`> pip install 'aif360[LFR,LIME,notebooks]==0.3.0rc0'`

Change to ~/Downloads/tutorial_files and run `python copy_datasets.py` to copy files into `/Applications/anaconda3/envs/aif360/lib/python3.7/site-packages/aif360/data/`.

For all functionality: `pip install 'aif360[all]==0.3.0rc0'`

Just in case: `> conda env remove --name aif360`

`> python -m ipykernel install --user --name aif360 --display-name "Python37 (aif360)"`

`> jupyter notebook`
