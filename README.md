# **United-States-Coal-Usage-Classification**
![Alt text](images/coal_seam_at_coal_mine.png)
An 80 foot coal seam at the North Antelope Rochelle opencut coal mine.<br>
By Peabody Energy, Inc. - Provided by Peabody Energy, CC BY 3.0, https://commons.wikimedia.org/w/index.php?curid=36846291

Overview
--------

This end-to-end machine learning project is focused on analyzing coal usage in the United States from 2001 to 2021 and classifying coal using data gathered from the U.S. Energy Information Administration (EIA) through their API. The data was cleaned and prepared for analysis using Geospatial Analysis, Chemometrics and coal production Time Series Analysis (only Trend). Custom Transformers were built for Feature Engineering. Transformation Pipelines were implemented for convenient preprocessing of data. Machine Learning algorithms like Softmax Regression, Decision Tree Classifier, Random Forest Classifier and Feed Forward Network were implemented and cross-validation was used to evaluate their performance. Hyperparameter Tuning was applied to improve the performance of Feed Forward Network. The Random Forest classification model was deployed using Flask on Render Cloud Hosting.

Table of contents
-----------------

1. Primary Objective
2. Results
3. Installation
4. Usage
5. Contributing
6. Credits
7. License
8. Contact

Primary Objective
-----------------

To analyze coal data provided by U.S. Energy Information Administration, build machine learning models that can classify coal based on parameters like heat content, ash content and sulphur content then deploy best performing model for educational purposes.

Results
-------

With performance measures like accuracy, precision, recall, and F1 score all greater than 99%, the classification model demonstrated outstanding results in its ability to accurately classify the data.

Installation
------------

**Prerequisites**:
  - Anaconda Python Distribution
  - python 3.9.16
  
Note: The steps below for installing packages involve 'requirements.txt' file. This file contains only those packages that were necessary for deployment of the flask app and therefore doesn't include all the packages that were used for the development of the project. 

1. **Install Conda**: If you do not have Conda installed on your system, you can download and install the appropriate version for your operating sytem from the official Conda Website (https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).
2. **Create an environment**: To avoid conflicts between packages, create a new environment. You can create one using the following command: `conda create -n ENVNAME python=3.9.16`. Replace `ENVNAME` with the name of your choice, for example: `coal-dep`, `coal-dev`.
3. **Activate the environment**: Once you have created the environment, you need to activate it to start using it. You can activate the environment using the following command: `conda activate ENVNAME`.
4. **Install packages**: You can now install the required packages in the environment using the either of the following commands:`conda install --yes --file requirements.txt` or `conda install --file requirements.txt`. The former automatically answers "yes" to all prompts during installation, while the latter requires user to manually confirm each installation prompt. If you're on a windows computer, you may have issues while running the above command because of gunicorn package. Since it is not needed for running an app locally, I recommend removing the 'gunicorn' package from requirements.txt file before running the command mentioned earlier in this step.
5. **Deactivate the environment**: Once you are done working with the environment, you can deactivate using `conda deactivate` and then close the prompt using `exit`.
That's it! You have now installed the packages using Conda.

Usage
-----

You can access the deployed project by following the link 'https://coal-rank-prediction-91cs.onrender.com/'. Alternatively, after installation you can also run the project locally by following the steps below:
1. Open Anaconda prompt.
2. Navigate to the project folder.
3. Run this command: `python main.py`.
4. Copy the url (http://localhost:5000 or similar) generated in the prompt.
5. Open a web browser and paste the url to access the web application.

Contributing
------------

Thank you for your interest in this project! At this time we are not accepting contribution from external collaborators. If you have any feedback or suggestions, please feel free to create an issue or contact us directly.

Credits
-------

- Data for this project was collected from the [U.S. Energy Information Administration (EIA)](https://www.eia.gov/) through their API.
- Images used in this project were sourced from:
  - Peabody Energy, Inc. - Provided by Peabody Energy, CC BY 3.0, https://commons.wikimedia.org/w/index.php?curid=36846291
  - James St. John - https://www.flickr.com/photos/47445767@N05/33554814475/, CC BY 2.0, https://commons.wikimedia.org/w/index.php?curid=95239731
  - James St. John - https://www.flickr.com/photos/jsjgeology/8512397381/in/album-72157632870063067/
  - Geos.berau - Own work, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=123014299
- Online flowchart tool - https://app.diagrams.net/

License
-------

This project is licensed under the [MIT License](LICENSE.txt) - see the [LICENSE.txt](LICENSE.txt) file for details.

Contact
-------

  - **Name**: Shreyas
  - **Email**: shreyasdb99@gmail.com
  - **GitHub**: [shre-db](https://github.com/shre-db)
  - **Instagram**: [shryzium](https://www.instagram.com/shryzium/)
