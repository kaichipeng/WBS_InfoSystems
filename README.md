<img width="1000" alt="portfolio_view" src="Images/wbs_lecture_infosystems.png">

---

Welcome to Warwick Bussiness School's Financial Technology, *Machine Learning Driven Quantitative Investment* Github repository. This repository is a unique resource containing expert led machine learning (ML) techniques, models and advanced approaches that are directly applied to stock selection in global equities. We have selected the best Python libraries to demonstrate how to drive machine learning approaches for equities selection and investment. Casuality is our bottom-line, and we take you on a journey from Granger causality, through to employing a ML toolkit cultminating in cutting edge XAI and mutli-task-machine-learning to get us to powerful, causal, explainable machine learning investment systems. 

We start our journey by loading our extensive dataset of financial reporting and exchange level data for several thousand global stocks across emerging and developed markets. We learn how to preprocess the data, impute, normalise and stack the information, ready for our learners. We touch on dimensionality reduction and show how old-style PCA has been improved upon by powerful neural, autoencoders. We take a short digression into Granger Causality as a foundation for the causality we want from our ML. Our learners start with OLS, ElasticNets, Random Forests, Artificial Neural Nets, before we get deep into cutting edge explainable AI (XAI). 

Explainability is crucial in finance and other domains where we are making critical decisions and those decisions may need to be scrutinised by clients, regulators, and ourselves for probable causality. We look at LIME and SHAP as XAI approaches to explain the working of black box learners. Finally we end on the advanced topic of mutli-task learning (MTL), one of the most powerful ways of achieving causal driven learning. 

This site contains the Python code for our module. The notebooks are designed to be self standing and can be worked through in your own time. The raw data that we will be using can be found in the [`Data`](Data) folder and is mainly anonymised data, with limited pertubations. 

## Contents 
  1. [loading_data.ipynb](https://github.com/danphilps/WBS_InfoSystems/blob/main/loading_data.ipynb) - For those of you that have downloaded the data in the XLSX format, this notebook shows you how we can use Python to automatically convert the worksheets in the XLSX into seperate CSV which are much faster to work with in Python.
  2. [preprocessing_pt1.ipynb](preprocessing_pt1.ipynb) - We formulate our problem... machine learning driven quanitative investing, extract the data, stack it, preprocess it and learn how to impute missing values.
  3. [preprocessing_pt2.ipynb](preprocessing_pt2.ipynb) - We learn how to deal with categorical data such as country, sector static info for our stocks, we touch on PCA to reduce the dimensionality of our dataset (thus making it much easier to pass into many learner types) and finish by looking at non-linear dimensionslity reduction by super powerful neural based auto-encoders.
  4. [time_series_forecasting_causality.ipynb](learners.ipynb) - We pause to look at simple techniques ot view our dataset and construct simple Econometric style time-series learners, concluding this notebook with Granger-causality. 
  5. [learners.ipynb](learners.ipynb) - Now the nitty gritty. Machine learning (ML) learners applied to our prepped dataset. We start with simple ordinary least squares regression (OLS) used to illustrate learner basics and to look at the weaknesses of OLS. The lesson is don't forget Econometrics, it will help in our machine learning. We progress to Regularisation, ElasticNets regresison, RandomForest, Neural nets. We then use XAI, explainable AI, using cutting edge tools to show how the outputs and dynamics of black box learners can be explained. LIME, SHAP are examined.   
  6. [MTL.ipynb](MTL.ipynb) - Finally we touch upon another cutting edge topic, multi-task-learning, where by learning multiple outcomes we can strengthen the results of our learners. We introduce a simple and cheap approach to MTL specific to finance that we have developed. 

We hope you enjoy our course and get loads out of it. 

## Downloading and running the code

The first step is to download the repository onto your computer. To do this click the green code button in top right of this page and click download as zip.

<img src="Images/download_repo.png" width=400px >

Once you have downloaded the zip folder put it into an appropriate place, right click the zip folder and click extract all. 

<img src="Images/extract_all.png" width=400px >

You should now have a folder called `WBS_InfoSystems-main` that contains all of the files and folders that you see in this repository. As mentioned before there are quite a lot of packages that have been used in this repository. To avoid any potential conflicts between packages you may have already installed we will install the packages needed for this repository in a new conda environment. Start by opening the anaconda command prompt. You should see a window similar to the one shown below.

<img src="Images/command_prompt.png" width=400px >

Now navigate to the `WBS_InfoSystems-main` folder using the `cd` command.

<img src="Images/navigate_to_folder.png" width=400px > 

Inside the `WBS_InfoSystems-main` folder, there is a file called `environment.yml` which contains the information needed to configure the conda environment. We can create a new environment based on `environment.yml` using the command `conda env create --name fintech --file=environment.yml` which creates an environment called fintech. Just a warning, installing all can take a while.

<img src="Images/create_env.png" width=600px >

After we have create the fintech environment, we can activate it using `conda activate fintech` and open jupyter notebook by simply typing `jupyter notebook`.

<img src="Images/open_notebook.png" width=400px >

Opening jupyter notebook from within the conda environment ensures that jupyter notebook is opened using the fintech environment. 

## Acknowledgements 
Thanks to Mr Alex Gregory for his significant contributions to the development of this programme.

## Owner details

### Dan Philps, PhD, CFA
<img src="Images/DGP.png" width=100px > 
Dr Dan Philps is head of Rothko Investment Strategies and is an artificial intelligence (AI) researcher. He has over 20 years of quantitative investment experience. Prior to Rothko, he was a senior portfolio manager at Mondrian Investment Partners. Before 1998, Philps worked at a number of major investment banks, specializing in the design/development of trading and risk models.
He holds a PhD in AI and Computer Science from City, University of London, a BSc (Hons) from King’s College London, is a CFA charterholder, a member of CFA Society of the UK and is a member of the AAAI.

### Prof Ram D. Gopal, PhD 
Prof Ram D. Gopal is the Information Systems Society’s Distinguished Fellow, a Professor of Information Systems Management, and Pro-Dean for Research, Engagement, and Impact at the Warwick Business School. He also serves as the Academic Director of the Gillmore Centre for Financial Technology at the Warwick Business School. He has a diverse and a rich portfolio of research that spans big data analytics, health informatics, financial technologies, information security, privacy and valuation, intellectual property rights, online market design and business impacts of technology.

### Alex Gregory
<img src="Images/picture[3187].jpg" width=100px > 
Mr Alex Gregory is an artificial intelligence (AI) researcher, and a Research Assistant at the University of Nottingham. Alex specialises in applying artificial intelligence to healthcare, with recent work using EEG data to predict neurological conditions. Alex has a BSc (Hons) in mathematics from University of Swansea and a MSc in artificial intelligence from Southampton University.
