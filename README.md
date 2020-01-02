# Football-Predictor

This is all the code and other work produced for my Cambridge University Computer Science Tripos Part II Project. The Project is titled "Predicting the Outcomes of English Premier League Matches".

Data is collected via web-scraping and manual collection where more appropriate. The data is transformed into a small set of features, used to build models that solve the following problem:

Given multiple features of an English Premier League match that can only be known before the game begins, predict the outcome of the match from the options {H,D,A}. H = Home Win, D = Draw, A = Away Win.

The goal is to exceed a 40% accuracy rate. Expert pundits Mark Lawrenson and Paul Merson achieve a predicition accuracy of ~52%, and exceeding this would make the project a very successful one.

## Getting Started

Replicating the results is not easily possible for obvious reasons. All csv files are not uploaded, all that is uploaded is the Code and the Deliverables. This is just a showcase of the work completed during the project.

Here I'll outline what each of the folders contains, which will help you quickly traverse to what you want to see. If you want to look through the code, I suggest reading this whole section, otherwise if you just want to see the Dissertation PDF that covers all work and rational behind the project, then skip to the section about the "Other" Folder.

### Adding Features

All code used for adding features to datasets during feature engineering. This includes generating new features, merging datasets of features and adding external features. Also includes some inevitable data cleaning. Additionally, code used to generate a full league table for each row of the dataset in included here.

### Data Backups - Not included in git

Worth mentioning here that I had a weekly backup of all code and files to both this folder and also an external drive.

### Data Cleaning and Fixing

Split by dataset/ data checkpoint, this includes all the code used to turn webscraped mess of datasets into a more compact and usable dataset. Also fixed missing values, inconsistencies and various other issues.

### Data Collecting

Split by source/ dataset, this includes code used to scrape thousands of pages from various websites to get all football results needed alongside lots of metadata associated with each match. For each website, there is a notebook used to figure out how to accurately scrape off of one page and get all the data needed, then another notebook that invokes that code on each of the thousands of pages needed, fixing bugs found along the way.

### Data Preparation for Models

Here is the code used to take the cleaned datasets and transform them into a model input, mainly by ensuring all features are numerical and creating a target variable. Various versions of data representation were tested to look for what works best with the models. Also includes majority of code used for league table generator and improvements made.

### Models

Includes all models built during the project. Includes an initial analysis phase too, where conclusions could be drawn on the dataset, the prediction systems to use and base goals to compare results to. Much more detail included in Dissertation PDF in the "Other" folder. Models are split by Spiral. During this project, I used a modified version of the Spiral Model from Software Development, tailored towards a data science project. This allowed me to take a dataset, build models for it, analyse the results, refine the data and models based on the analysis and then repeat. Again, this is explained more clearly in the Dissertation PDF. Models include simple Neural Nets, KNN's, Naive Bayes and more, and even some more complex NN's with multiple hidden layers. All models, results and analysis detailed in Dissertation PDF.

### Other

Includes all Deliverables made during the project. The Project Proposal was made before the project began, outline my ideas and goals. The Progress Report outlined an almost-halfway update, detailing work completed so far and future goals. The Final Dissertation is my entire final submission, detailing the entire project including research, initial goals, developments, all work completed and conclusions. Not included in git but also in this folder was all figures, organisation files (todo's, work completed trackers, etc), and all temporary code.

## Built With

* [Anaconda](https://www.anaconda.com/distribution/#download-section) - Includes Jupyter Notebooks, Python (3+ will work) and many typically used Python Packages. Linux Distribution.

## Authors

* **Joseph Marchant** - *All work* - [joecode0](https://github.com/joecode0)

