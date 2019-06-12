# Introduction to machine learning with Python and Azure Notebooks



# PART 1: Analyze climate data with Azure Notebooks



# Introduction

- 5 minutes

Azure Notebooks is a cloud-based platform for building and running [Jupyter](http://jupyter.org/) notebooks. Jupyter is an environment based on [IPython](https://ipython.org/) that facilitates interactive programming and data analysis using a variety of programming languages, including Python. Jupyter notebooks enjoy widespread use in research and academia for mathematical modeling, machine learning, statistical analysis, and for teaching and learning how to code.

Azure Notebooks provide Jupyter as a service for free. It's a convenient way to build notebooks and share them with others without having to install and manage a Jupyter server. And it's web-based, making it an ideal solution for collaborating online. In this lab, you will create an Azure Notebook and use three popular Python libraries — [scikit-learn](http://scikit-learn.org/stable/index.html), [NumPy](http://www.numpy.org/), and [Seaborn](https://seaborn.pydata.org/) — to analyze climate data collected by NASA. Then you will share the notebook so others can experiment with it, too.

## Learning objectives

In this lab, you will:

- Create a notebook in Azure Notebooks
- Upload, manipulate, and visualize data in a notebook
- Share notebooks online

------

## Next unit: Create an Azure Notebook

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/1-create-an-azure-notebook)










# Create an Azure Notebook

- 5 minutes

The first order of business is to create a new Azure Notebook. Azure Notebooks are contained in *libraries* whose primary purpose is to group related notebooks. In this unit, you'll create a new project and then create a notebook inside it.

1. Navigate to [https://notebooks.azure.com ](https://notebooks.azure.com/) in your browser.

2. Sign in using your Microsoft account.

3. Click **My Projects** in the top menubar.

   ![Navigating to the Projects page](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/1-add-project-1.png)

   *Navigating to the Projects page*

4. Click **+ New Project**. Enter "Climate Change" (without quotation marks) for the project name and "climate-change" as the project ID. Uncheck the **Public project** box, and then click **Create**.

   ![Creating a project](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/1-add-project-2.png)

   *Creating a project*

5. Click the **+** sign to add a notebook to the project.

   ![Adding a notebook to the project](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/1-add-notebook-1.png)

   *Adding a notebook to the project*

6. Name the notebook "climatechange.ipynb" and select **Python 3.6 Notebook** as the item type. This will create a notebook with a Python 3.6 kernel. One of the strengths of Jupyter notebooks is that you can use different languages by choosing different kernels.

   ![Creating a notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/1-add-notebook-2.png)

   *Creating a notebook*

   If you're curious, the **.ipynb** file-name extension stands for "IPython notebook." Jupyter notebooks were originally known as IPython (Interactive Python) notebooks, and they only supported Python as a programming language. The name Jupyter is a combination of Julia, Python, and R — the core programming languages that Jupyter supports.

7. Click the new notebook. This will launch the notebook and allow you to start editing it.

   ![Opening the notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/1-open-notebook.png)

   *Opening the notebook*

You can create additional projects and notebooks as you work with Azure Notebooks. Projects provide a means for grouping related notebooks. You can create notebooks from scratch, or you can upload existing notebooks. In the next unit, you'll build a notebook from scratch and learn the basics of working with cells.

------

## Next unit: Upload Data and Create Scatterplot

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/2-upload-data-and-create-scatterplot)











# Upload Data and Create Scatterplot

- 5 minutes

Jupyter notebooks are composed of *cells*. Each cell is assigned one of three types:

- **Markdown** for entering text in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) format
- **Code** for entering code that runs interactively
- **Raw NBConvert** for entering data inline

Code entered into code cells is executed by a *kernel*, which provides an isolated environment for the notebook to run in. The popular IPython kernel supports code written in Python, but [dozens of other kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels) are available supporting other languages. Azure Notebooks support Python, R, and F# out of the box. They also support the installation of the many packages and libraries that are commonly used in research.

The notebook editor currently shows an empty cell. In this exercise, you will add content to that cell and add other cells to import Python packages such as [NumPy](http://www.numpy.org/), load a pair of NASA data files containing [climate data](https://data.giss.nasa.gov/gistemp/graphs_v3/), and create a scatter plot from the data.

1. In the first cell, set the cell type to **Markdown** and enter the "Azure Notebook Climate Change Analysis" into the cell itself:

   ![Defining a markdown cell](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-jupyter-1.png)

   *Defining a markdown cell*

2. Click the **+** button in the toolbar to add a new cell. Make sure the cell type is **Code**, and then enter the following Python code into the cell:

   PythonCopy

   ```python
   import matplotlib.pyplot as plt
   import numpy as np
   from sklearn.linear_model import LinearRegression
   import seaborn as sns; sns.set()
   ```

   ![Adding a code cell](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-jupyter-2.png)

   *Adding a code cell*

3. Now click the **Run** button to run the code cell and import the packages specified in the `import` statements. Ignore any warnings that are displayed as the environment is prepared for the first time.

   > You can remove the warnings by selecting the code cell and running it again.

   ![Running a code cell](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-jupyter-3.png)

   *Running a code cell*

4. Click **File** in the menu at the top of the page, and select **Upload** from the drop-down menu. Then upload the files named **5-year-mean-1951-1980.csv** and **5-year-mean-1882-2014.csv** from [this link](https://a4r.blob.core.windows.net/public/notebook-resources.zip).

   ![Uploading data to the notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-upload-data.png)

   *Uploading data to the notebook*

5. Select **/project** as your **Destination Folder** to ensure your files persist. Click **Start Upload** to upload the files, and **OK**once they successfully upload.

   ![Selecting destination folder for data](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-destination-folder.png)

   *Selecting destination folder for data*

6. Place the cursor in the empty cell at the bottom of the notebook. Enter "Import data" as the text and change the cell type to **Markdown**.

7. Now add a **Code** cell and paste in the following code.

   PythonCopy

   ```python
   yearsBase, meanBase = np.loadtxt('5-year-mean-1951-1980.csv', delimiter=',', usecols=(0, 1), unpack=True)
   years, mean = np.loadtxt('5-year-mean-1882-2014.csv', delimiter=',', usecols=(0, 1), unpack=True)
   ```

8. Click the **Run** button to run the cell and use NumPy's `loadtxt` function to load the data that you uploaded. The data is now in memory and can be used by the application.

   ![Loading the data](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-jupyter-4.png)

   *Loading the data*

9. Place the cursor in the empty cell at the bottom of the notebook. Change the cell type to **Markdown** and enter "Create a scatter plot" as the text.

10. Add a **Code** cell and paste in the following code, which uses [Matplotlib](http://matplotlib.org/) to create a scatter plot.

    PythonCopy

    ```python
    plt.scatter(yearsBase, meanBase)
    plt.title('scatter plot of mean temp difference vs year')
    plt.xlabel('years', fontsize=12)
    plt.ylabel('mean temp difference', fontsize=12)
    plt.show()
    ```

11. Click **Run** to run the cell and create a scatter plot.

    ![Scatter plot produced by Matplotlib](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/2-scatter-plot.png)

    *Scatter plot produced by Matplotlib*

The data set you loaded uses a 30-year mean between 1951 and 1980 to calculate a base temperature for that period, and then uses 5-year mean temperatures to calculate the difference between the 5-year mean and the 30-year mean for each year. The scatter plot shows the annual temperature differences.

------

## Next unit: Perform Linear Regression with Numpy

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/3-perform-linear-regression-with-numpy)









# Perform Linear Regression with Numpy

- 5 minutes

Scatter plots offer a handy means for visualizing data, but suppose you wanted to overlay the scatter plot with a trend line showing how the data is trending over time. One way to compute such trend lines is [linear regression](https://en.wikipedia.org/wiki/Linear_regression). In this exercise, you will use NumPy to perform a linear regression and Matplotlib to draw a trend line from the data.

1. Place the cursor in the empty cell at the bottom of the notebook. Change the cell type to **Markdown** and enter "Perform linear regression" as the text.

2. Add a **Code** cell and paste in the following code. Take a moment to read the comments (the lines that begin with # signs) to understand what the code is doing.

   PythonCopy

   ```python
   # Creates a linear regression from the data points
   m,b = np.polyfit(yearsBase, meanBase, 1)
   
   # This is a simple y = mx + b line function
   def f(x):
       return m*x + b
   
   # This generates the same scatter plot as before, but adds a line plot using the function above
   plt.scatter(yearsBase, meanBase)
   plt.plot(yearsBase, f(yearsBase))
   plt.title('scatter plot of mean temp difference vs year')
   plt.xlabel('years', fontsize=12)
   plt.ylabel('mean temp difference', fontsize=12)
   plt.show()
   
   # Prints text to the screen showing the computed values of m and b
   print(' y = {0} * x + {1}'.format(m, b))
   plt.show()
   ```

3. Now run the cell to display a scatter plot with a regression line.

   ![Scatter plot with regression line](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/3-num-py-regression.png)

   *Scatter plot with regression line*

From the regression line, you can see that the difference between 30-year mean temperatures and 5-year mean temperatures is increasing over time. Most of the computational work required to generate the regression line was done by NumPy's `polyfit` function, which computed the values of `m` and `b` in the equation y = mx + b.

------

## Next unit: Perform Linear Regression with Scikit Learn

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/4-perform-linear-regression-with-scikit-learn)








# Perform Linear Regression with Scikit Learn

- 5 minutes

Another popular Python library that is widely used in the research community is [scikit-learn](http://scikit-learn.org/stable/), which excels at building machine-learning models to help extract information from data. In this exercise, you will use scikit-learn (which was already imported in Unit 2) to compute a trend line for the NASA climate data.

1. Place the cursor in the empty cell at the bottom of the notebook. Change the cell type to **Markdown** and enter "Perform linear regression with scikit-learn" as the text.

2. Add a **Code** cell and paste in the following code.

   PythonCopy

   ```python
   # Pick the Linear Regression model and instantiate it
   model = LinearRegression(fit_intercept=True)
   
   # Fit/build the model
   model.fit(yearsBase[:, np.newaxis], meanBase)
   mean_predicted = model.predict(yearsBase[:, np.newaxis])
   
   # Generate a plot like the one in the previous exercise
   plt.scatter(yearsBase, meanBase)
   plt.plot(yearsBase, mean_predicted)
   plt.title('scatter plot of mean temp difference vs year')
   plt.xlabel('years', fontsize=12)
   plt.ylabel('mean temp difference', fontsize=12)
   plt.show()
   
   print(' y = {0} * x + {1}'.format(model.coef_[0], model.intercept_))
   ```

3. Now run the cell to display a scatter plot with a regression line.

   ![Scatter plot with regression line computed by sckikit-learn](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/4-sklearn-regression.png)

   *Scatter plot with regression line computed by sckikit-learn*

The output is almost identical to the output in the previous exercise. The difference is that scikit-learn did more of the work for you. Specifically, you didn't have to code a line function as you did with NumPy; scikit-learn's `LinearRegression`function did it for you. scikit-learn supports *many* different types of regression, which comes in handy when building sophisticated machine-learning models.

------

## Next unit: Analyze Data with Seaborn

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/5-analyze-data-with-seaborn)









# Analyze Data with Seaborn

- 5 minutes

One of the cool things about Azure Notebooks — and Python in general — is there are thousands of open-source libraries you can leverage to perform complex tasks without writing a lot of code. In this unit, you'll use [Seaborn](https://seaborn.pydata.org/), a library for statistical visualization, to plot the second of the two data sets you loaded, which covers the years 1882 to 2014. Seaborn can create a regression line accompanied by a projection showing where data points should fall based on the regression with one simple function call.

1. Place the cursor in the empty cell at the bottom of the notebook. Change the cell type to **Markdown** and enter "Perform linear regression with Seaborn" as the text.

2. Add a **Code** cell and paste in the following code.

   PythonCopy

   ```python
   plt.scatter(years, mean)
   plt.title('scatter plot of mean temp difference vs year')
   plt.xlabel('years', fontsize=12)
   plt.ylabel('mean temp difference', fontsize=12)
   sns.regplot(yearsBase, meanBase)
   plt.show()
   ```

3. Run the code cell to produce a scatter chart with a regression line *and* a visual representation of the range in which the data points are expected to fall.

   ![Comparison of actual values and predicted values generated with Seaborn](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/5-seaborn-regression.png)

   *Comparison of actual values and predicted values generated with Seaborn*

Notice how the data points for the first 100 years conform nicely to the predicted values, but the data points from roughly 1980 forward don't. It's models such as these that lead scientists to believe that climate change is accelerating.

------

## Next unit: Share a Notebook

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/7-share-a-notebook)









# Share a Notebook

- 5 minutes

One of the value-added features of Azure Notebooks is that it provides a cloud-based hub for sharing notebooks. In this unit, you'll share the notebook you created in previous exercises.

1. Select **File** -> **Close and Halt** to close the notebook.

   ![Closing the notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/7-share-1.png)

   *Closing the notebook*

2. Click **Project Settings** to edit the project's settings. Check the **Public project** box to make the project public, and then click **Save**.

   ![Making the project public](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/7-share-2.png)

   *Making the project public*

3. Click **Share**. Notebooks can be shared by links, on social media, and through email. To demonstrate, click **Copy Link**to copy a link to the notebook to the clipboard. Then paste the link into a separate browser window and confirm that the notebook appears there.

   ![Sharing by link](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-climate-data-with-azure-notebooks/media/7-share-3.png)

   *Sharing by link*

Another way to share a notebook is to download it as a **.ipynb** file and send the **.ipynb** file to whomever you wish to share it with. You can download a notebook and make a local copy by clicking the **Download Project** button. You can even run them in other Jupyter environments if you would like because there's nothing proprietary about Azure Notebooks.

------

## Next unit: Summary and knowledge check

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-climate-data-with-azure-notebooks/8-summary-and-knowledge-check)









# Summary and knowledge check

- 10 minutes

There's much more to do and learn with Azure Notebooks, like integrate with Azure Machine Learning, and connect the notebook to your own Azure compute source. The Azure Notebooks Web site contains several sample notebooks that you can experiment with and learn from. Here are two great examples.

- [Discover Sentiments in Tweets](https://notebooks.azure.com/Microsoft/libraries/samples/html/Discover Sentiments in Tweets.ipynb) performs sentiment analysis on 160,000 tweets, and uses the [word_cloud](https://github.com/amueller/word_cloud) package to generate word clouds from the tweets.
- [Introduction to Cognitive Toolkit](https://notebooks.azure.com/cntk/libraries/tutorials) is a library of notebooks that demonstrate how to use the [Microsoft Cognitive Toolkit](https://www.microsoft.com/research/product/cognitive-toolkit/) to build sophisticated machine-learning models.

Check out the Azure Notebooks home page for additional sample notebooks, and use them to deepen your understanding of Jupyter and sharpen your data-science skills.

## Learn more

- [Azure Notebooks Web site](https://notebooks.azure.com/)
- [Azure Notebooks documentation](https://docs.microsoft.com/azure/notebooks/)
- [Azure Notebooks samples](https://github.com/Microsoft/AzureNotebooks)

## Check your knowledge

\1. 

What is a strength of using Jupyter Notebooks?



Can use different databases by choosing different kernels.



Can use different languages by choosing different kernels.



Can use different themes by choosing different kernels.

\2. 

What kind of line can a linear regression help create?



Differentiation



Slope



Trend

\3. 

What types of cells can you have in a Jupyter notebook?



Markdown and Code



Editable and Uneditable



Markdown, Code, and Raw NBConvert









# PART 2: Predict flight delays by creating a machine learning model in Python

# Introduction

- 5 minutes

Python is one of the world's most popular programming languages. It's used extensively in the data science community for machine learning and statistical analysis. One of the reasons it's so popular is the availability of thousands of open-source libraries such as NumPy, Pandas, Matplotlib, and scikit-learn, which enable programmers and researchers alike to explore, transform, analyze, and visualize data.

Azure Notebooks is a cloud-based platform for building and running Jupyter notebooks. Jupyter is an environment based on IPython that facilitates interactive programming and data analysis using Python and other programming languages. Azure Notebooks provide Jupyter as a service for free. It's a convenient way to write Python code without having to install and manage a Jupyter server. And it's web-based, making it an ideal solution for collaborating online.

In this module, you'll create an Azure Notebook, import a dataset containing on-time arrival information for a major U.S. airline, and load the dataset into the notebook. Then, you'll clean the dataset with Pandas, build a machine-learning model with scikit-learn, and use Matplotlib to visualize output from the model.

## Learning Objectives

In this module, you will:

- Create a Jupyter notebook in Azure Notebooks, import data, and view data loaded into the notebook.
- Use Pandas to clean and prepare data to be used for the machine-learning model.
- Use scikit-learn to create the machine learning model.
- Use Matplotlib to visualize the model's performance.

------

## Next unit: Create an Azure Notebook and Import Data

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-flight-delays-with-python/1-create-notebook-and-import-data)









# Create an Azure Notebook and Import Data

- 8 minutes

The first order of business is to create a new Azure notebook. Azure notebooks are contained in projects, whose primary purpose is to group related notebooks. In this unit, you'll create a new project and then create a notebook inside it.

1. Navigate to [https://notebooks.azure.com ](https://notebooks.azure.com/) in your browser

2. Sign in using your Microsoft account.

3. Click **My Projects** in the menu at the top of the page.

4. Click the **+ New Project** button at the top of the "My Projects" page.

5. Create a new project named "ML Notebooks" or something similar. You may uncheck the "Public" box if you'd like, but making the project public allows the notebooks in it to be shared with others through links, social media, or e-mail. If you're unsure which to choose, you can easily change a project to public or private later on.

   ![Creating a project](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-add-project.png)

   *Creating a project*

6. Click **+ New** and select **Notebook** from the menu to add a notebook to the project.

   ![Adding a notebook to the project](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-add-notebook-1.png)

   *Adding a notebook to the project*

7. Give the notebook a name such as "On-Time Flight Arrivals.ipynb," and select **Python 3.6** as the language. This will create a notebook with a Python 3.6 kernel for executing Python code. One of the strengths of Azure notebooks is that you can use different languages by choosing different kernels.

   ![Creating a notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-add-notebook-2.png)

   *Creating a notebook*

   If you're curious, the **.ipynb** file-name extension stands for "IPython notebook." Jupyter notebooks were originally known as IPython (Interactive Python) notebooks, and they only supported Python as a programming language. The name Jupyter is a combination of Julia, Python, and R — the core programming languages that Jupyter supports.

8. Click the notebook to open it for editing.

   ![Opening the notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-open-notebook.png)

   *Opening the notebook*

You can create additional projects and notebooks as you work with Azure Notebooks. You can create notebooks from scratch, or you can upload existing notebooks.

Jupyter notebooks are highly interactive, and since they can include executable code, they provide the perfect platform for manipulating data and building predictive models from it.

1. Enter the following command into the first cell of the notebook:

   bashCopy

   ```bash
   !curl https://topcs.blob.core.windows.net/public/FlightData.csv -o flightdata.csv
   ```

    Tip

   `curl` is a Bash command. You can execute Bash commands in a Jupyter notebook by prefixing them with an exclamation mark. This command downloads a CSV file from Azure blob storage and saves it using the name **flightdata.csv**.

2. Click the **Run** button to execute the `curl` command.

   ![Importing a dataset](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-import-dataset.png)

   *Importing a dataset*

3. In the notebook's second cell, enter the following Python code to load **flightdata.csv**, create a [Pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html)from it, and display the first five rows.

   PythonCopy

   ```python
   import pandas as pd
   
   df = pd.read_csv('flightdata.csv')
   df.head()
   ```

4. Click the **Run** button to execute the code. Confirm that the output resembles the output below.

   ![Loading the dataset](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/1-load-dataset.png)

   *Loading the dataset*

   The **DataFrame** that you created contains on-time arrival information for a major U.S. airline. It has more than 11,000 rows and 26 columns. (The output says "5 rows" because DataFrame's [head](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.head.html) function only returns the first five rows.) Each row represents one flight and contains information such as the origin, the destination, the scheduled departure time, and whether the flight arrived on time or late. We'll look at the data more closely a bit later in this module.

5. Use the **File** -> **Save and Checkpoint** command to save the notebook.

Use the horizontal scroll bar to scroll left and right and view all the columns in the dataset. How many columns does the dataset contain? Can you guess what each column represents from the column names?

------

## Next unit: Clean and Prepare Data

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-flight-delays-with-python/2-clean-and-prepare-data)











# Clean and Prepare Data

- 10 minutes

Before you can prepare a dataset, you need to understand its content and structure. In the previous lab, you imported a dataset containing on-time arrival information for a major U.S. airline. That data included 26 columns and thousands of rows, with each row representing one flight and containing information such as the flight's origin, destination, and scheduled departure time. You also loaded the data into a Jupyter notebook and used a simple Python script to create a Pandas DataFrame from it.

A [DataFrame](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html) is a two-dimensional labeled data structure. The columns in a DataFrame can be of different types, just like columns in a spreadsheet or database table. It is the most commonly used object in Pandas. In this exercise, you will examine the DataFrame — and the data inside it — more closely.

1. Switch back to the Azure notebook that you created in the previous section. If you closed the notebook, you can sign back into the [Microsoft Azure Notebooks portal ](https://notebooks.azure.com/), open your notebook and use the **Cell** -> **Run All** to rerun the all of the cells in the notebook after opening it.

   ![The FlightData notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-load-dataset.png)

   *The FlightData notebook*

2. The code that you added to the notebook in the previous lab creates a DataFrame from **flightdata.csv** and calls [DataFrame.head](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.head.html) on it to display the first five rows. One of the first things you typically want to know about a dataset is how many rows it contains. To get a count, type the following statement into an empty cell at the end of the notebook and run it:

   PythonCopy

   ```python
   df.shape
   ```

   Confirm that the DataFrame contains 11,231 rows and 26 columns:

   ![Getting a row and column count](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-shape-output.png)

   *Getting a row and column count*

3. Now take a moment to examine the 26 columns in the dataset. They contain important information such as the date that the flight took place (YEAR, MONTH, and DAY_OF_MONTH), the origin and destination (ORIGIN and DEST), the scheduled departure and arrival times (CRS_DEP_TIME and CRS_ARR_TIME), the difference between the scheduled arrival time and the actual arrival time in minutes (ARR_DELAY), and whether the flight was late by 15 minutes or more (ARR_DEL15).

   Here is a complete list of the columns in the dataset. Times are expressed in 24-hour military time. For example, 1130 equals 11:30 a.m. and 1500 equals 3:00 p.m.

   | Column              | Description                                                  |
   | :------------------ | :----------------------------------------------------------- |
   | YEAR                | Year that the flight took place                              |
   | QUARTER             | Quarter that the flight took place (1-4)                     |
   | MONTH               | Month that the flight took place (1-12)                      |
   | DAY_OF_MONTH        | Day of the month that the flight took place (1-31)           |
   | DAY_OF_WEEK         | Day of the week that the flight took place (1=Monday, 2=Tuesday, etc.) |
   | UNIQUE_CARRIER      | Airline carrier code (e.g., DL)                              |
   | TAIL_NUM            | Aircraft tail number                                         |
   | FL_NUM              | Flight number                                                |
   | ORIGIN_AIRPORT_ID   | ID of the airport of origin                                  |
   | ORIGIN              | Origin airport code (ATL, DFW, SEA, etc.)                    |
   | DEST_AIRPORT_ID     | ID of the destination airport                                |
   | DEST                | Destination airport code (ATL, DFW, SEA, etc.)               |
   | CRS_DEP_TIME        | Scheduled departure time                                     |
   | DEP_TIME            | Actual departure time                                        |
   | DEP_DELAY           | Number of minutes departure was delayed                      |
   | DEP_DEL15           | 0=Departure delayed less than 15 minutes, 1=Departure delayed 15 minutes or more |
   | CRS_ARR_TIME        | Scheduled arrival time                                       |
   | ARR_TIME            | Actual arrival time                                          |
   | ARR_DELAY           | Number of minutes flight arrived late                        |
   | ARR_DEL15           | 0=Arrived less than 15 minutes late, 1=Arrived 15 minutes or more late |
   | CANCELLED           | 0=Flight was not cancelled, 1=Flight was cancelled           |
   | DIVERTED            | 0=Flight was not diverted, 1=Flight was diverted             |
   | CRS_ELAPSED_TIME    | Scheduled flight time in minutes                             |
   | ACTUAL_ELAPSED_TIME | Actual flight time in minutes                                |
   | DISTANCE            | Distance traveled in miles                                   |

The dataset includes a roughly even distribution of dates throughout the year, which is important because a flight out of Minneapolis is less likely to be delayed due to winter storms in July than it is in January. But this dataset is far from being "clean" and ready to use. Let's write some Pandas code to clean it up.

One of the most important aspects of preparing a dataset for use in machine learning is selecting the "feature" columns that are relevant to the outcome you are trying to predict while filtering out columns that do not affect the outcome, could bias it in a negative way, or might produce [multicollinearity](https://en.wikipedia.org/wiki/Multicollinearity). Another important task is to eliminate missing values, either by deleting the rows or columns containing them or replacing them with meaningful values. In this exercise, you will eliminate extraneous columns and replace missing values in the remaining columns.

1. One of the first things data scientists typically look for in a dataset is missing values. There's an easy way to check for missing values in Pandas. To demonstrate, execute the following code in a cell at the end of the notebook:

   PythonCopy

   ```python
   df.isnull().values.any()
   ```

   Confirm that the output is "True," which indicates that there is at least one missing value somewhere in the dataset.

   ![Checking for missing values](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-check-for-missing-values.png)

   *Checking for missing values*

2. The next step is to find out where the missing values are. To do so, execute the following code:

   PythonCopy

   ```python
   df.isnull().sum()
   ```

   Confirm that you see the following output listing a count of missing values in each column:

   ![Number of missing values in each column](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-count-missing-values.png)

   *Number of missing values in each column*

3. Curiously, the 26th column ("Unnamed: 25") contains 11,231 missing values, which equals the number of rows in the dataset. This column was mistakenly created because the CSV file that you imported contains a comma at the end of each line. To eliminate that column, add the following code to the notebook and execute it:

   PythonCopy

   ```python
   df = df.drop('Unnamed: 25', axis=1)
   df.isnull().sum()
   ```

   Inspect the output and confirm that column 26 has disappeared from the DataFrame:

   ![The DataFrame with column 26 removed](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-phantom-column-removed.png)

   *The DataFrame with column 26 removed*

4. The DataFrame still contains a lot of missing values, but some of them aren't useful because the columns containing them are not relevant to the model that you are building. The goal of that model is to predict whether a flight you are considering booking is likely to arrive on time. If you know that the flight is likely to be late, you might choose to book another flight.

   The next step, therefore, is to filter the dataset to eliminate columns that aren't relevant to a predictive model. For example, the aircraft's tail number probably has little bearing on whether a flight will arrive on time, and at the time you book a ticket, you have no way of knowing whether a flight will be cancelled, diverted, or delayed. By contrast, the scheduled departure time could have a *lot* to do with on-time arrivals. Because of the hub-and-spoke system used by most airlines, morning flights tend to be on time more often than afternoon or evening flights. And at some major airports, traffic stacks up during the day, increasing the likelihood that later flights will be delayed.

   Pandas provides an easy way to filter out columns you don't want. Execute the following code in a new cell at the end of the notebook:

   PythonCopy

   ```python
   df = df[["MONTH", "DAY_OF_MONTH", "DAY_OF_WEEK", "ORIGIN", "DEST", "CRS_DEP_TIME", "ARR_DEL15"]]
   df.isnull().sum()
   ```

   The output shows that the DataFrame now includes only the columns that are relevant to the model, and that the number of missing values is greatly reduced:

   ![The filtered DataFrame](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-reduced-columns.png)

   *The filtered DataFrame*

5. The only column that now contains missing values is the ARR_DEL15 column, which uses 0s to identify flights that arrived on time and 1s for flights that didn't. Use the following code to show the first five rows with missing values:

   PythonCopy

   ```python
   df[df.isnull().values.any(axis=1)].head()
   ```

   Pandas represents missing values with `NaN`, which stands for *Not a Number*. The output shows that these rows are indeed missing values in the ARR_DEL15 column:

   ![Rows with missing values](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-rows-with-missing-values.png)

   *Rows with missing values*

6. The reason these rows are missing ARR_DEL15 values is that they all correspond to flights that were canceled or diverted. You could call [dropna](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.dropna.html) on the DataFrame to remove these rows. But since a flight that is canceled or diverted to another airport could be considered "late," let's use the [fillna](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.fillna.html) method to replace the missing values with 1s.

   Use the following code to replace missing values in the ARR_DEL15 column with 1s and display rows 177 through 184:

   PythonCopy

   ```python
   df = df.fillna({'ARR_DEL15': 1})
   df.iloc[177:185]
   ```

   Confirm that the `NaN`s in rows 177, 179, and 184 were replaced with 1s indicating that the flights arrived late:

   ![NaNs replaced with 1s](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-missing-values-filled.png)

   *NaNs replaced with 1s*

The dataset is now "clean" in the sense that missing values have been replaced and the list of columns has been narrowed to those most relevant to the model. But you're not finished yet. There is more to do to prepare the dataset for use in machine learning.

The CRS_DEP_TIME column of the dataset you are using represents scheduled departure times. The granularity of the numbers in this column — it contains more than 500 unique values — could have a negative impact on accuracy in a machine-learning model. This can be resolved using a technique called [binning](http://data-informed.com/enhance-machine-learning-with-standardizing-binning-reducing/) or quantization. What if you divided each number in this column by 100 and rounded down to the nearest integer? 1030 would become 10, 1925 would become 19, and so on, and you would be left with a maximum of 24 discrete values in this column. Intuitively, it makes sense, because it probably doesn't matter much whether a flight leaves at 10:30 a.m. or 10:40 a.m. It matters a great deal whether it leaves at 10:30 a.m. or 5:30 p.m.

In addition, the dataset's ORIGIN and DEST columns contain airport codes that represent categorical machine-learning values. These columns need to be converted into discrete columns containing indicator variables, sometimes known as "dummy" variables. In other words, the ORIGIN column, which contains five airport codes, needs to be converted into five columns, one per airport, with each column containing 1s and 0s indicating whether a flight originated at the airport that the column represents. The DEST column needs to be handled in a similar manner.

In this exercise, you will "bin" the departure times in the CRS_DEP_TIME column and use Pandas' [get_dummies](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.get_dummies.html) method to create indicator columns from the ORIGIN and DEST columns.

1. Use the following command to display the first five rows of the DataFrame:

   PythonCopy

   ```python
   df.head()
   ```

   Observe that the CRS_DEP_TIME column contains values from 0 to 2359 representing military times.

   ![The DataFrame with unbinned departure times](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-unbinned-departure-times.png)

   *The DataFrame with unbinned departure times*

2. Use the following statements to bin the departure times:

   PythonCopy

   ```python
   import math
   
   for index, row in df.iterrows():
       df.loc[index, 'CRS_DEP_TIME'] = math.floor(row['CRS_DEP_TIME'] / 100)
   df.head()
   ```

   Confirm that the numbers in the CRS_DEP_TIME column now fall in the range 0 to 23:

   ![The DataFrame with binned departure times](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-binned-departure-times.png)

   *The DataFrame with binned departure times*

3. Now use the following statements to generate indicator columns from the ORIGIN and DEST columns, while dropping the ORIGIN and DEST columns themselves:

   PythonCopy

   ```python
   df = pd.get_dummies(df, columns=['ORIGIN', 'DEST'])
   df.head()
   ```

   Examine the resulting DataFrame and observe that the ORIGIN and DEST columns were replaced with columns corresponding to the airport codes present in the original columns. The new columns have 1s and 0s indicating whether a given flight originated at or was destined for the corresponding airport.

   ![The DataFrame with indicator columns](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/2-categorical-columns.png)

   *The DataFrame with indicator columns*

4. Use the **File** -> **Save and Checkpoint** command to save the notebook.

The dataset looks very different than it did at the start, but it is now optimized for use in machine learning.

------

## Next unit: Build Machine Learning Model

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-flight-delays-with-python/3-build-machine-learning-model)







# Build Machine Learning Model

- 15 minutes

To create a machine learning model, you need two datasets: one for training and one for testing. In practice, you often have only one dataset, so you split it into two. In this exercise, you will perform an 80-20 split on the DataFrame you prepared in the previous lab so you can use it to train a machine learning model. You will also separate the DataFrame into feature columns and label columns. The former contains the columns used as input to the model (for example, the flight's origin and destination and the scheduled departure time), while the latter contains the column that the model will attempt to predict — in this case, the ARR_DEL15 column, which indicates whether a flight will arrive on time.

1. Switch back to the Azure notebook that you created in the previous section. If you closed the notebook, you can sign back into the [Microsoft Azure Notebooks portal ](https://notebooks.azure.com/), open your notebook, and use the **Cell** -> **Run All** to rerun the all of the cells in the notebook after opening it.

2. In a new cell at the end of the notebook, enter and execute the following statements:

   PythonCopy

   ```python
   from sklearn.model_selection import train_test_split
   train_x, test_x, train_y, test_y = train_test_split(df.drop('ARR_DEL15', axis=1), df['ARR_DEL15'], test_size=0.2, random_state=42)
   ```

   The first statement imports scikit-learn's [train_test_split](http://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) helper function. The second line uses the function to split the DataFrame into a training set containing 80% of the original data, and a test set containing the remaining 20%. The `random_state` parameter seeds the random-number generator used to do the splitting, while the first and second parameters are DataFrames containing the feature columns and the label column.

3. `train_test_split` returns four DataFrames. Use the following command to display the number of rows and columns in the DataFrame containing the feature columns used for training:

   PythonCopy

   ```python
   train_x.shape
   ```

4. Now use this command to display the number of rows and columns in the DataFrame containing the feature columns used for testing:

   PythonCopy

   ```python
   test_x.shape
   ```

   How do the two outputs differ, and why?

Can you predict what you would see if you called `shape` on the other two DataFrames, `train_y` and `test_y`? If you're not sure, try it and find out.

There are many types of machine learning models. One of the most common is the regression model, which uses one of a number of regression algorithms to produce a numeric value — for example, a person's age or the probability that a credit-card transaction is fraudulent. You'll train a classification model, which seeks to resolve a set of inputs into one of a set of known outputs. A classic example of a classification model is one that examines e-mails and classifies them as "spam" or "not spam." Your model will be a binary classification model that predicts whether a flight will arrive on-time or late ("binary" because there are only two possible outputs).

One of the benefits of using scikit-learn is that you don't have to build these models — or implement the algorithms that they use — by hand. Scikit-learn includes a variety of classes for implementing common machine learning models. One of them is [RandomForestClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html), which fits multiple decision trees to the data and uses averaging to boost the overall accuracy and limit [overfitting](https://en.wikipedia.org/wiki/Overfitting).

1. Execute the following code in a new cell to create a `RandomForestClassifier` object and train it by calling the [fit](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier.fit)method.

   PythonCopy

   ```python
   from sklearn.ensemble import RandomForestClassifier
   
   model = RandomForestClassifier(random_state=13)
   model.fit(train_x, train_y)
   ```

   The output shows the parameters used in the classifier, including `n_estimators`, which specifies the number of trees in each decision-tree forest, and `max_depth`, which specifies the maximum depth of the decision trees. The values shown are the defaults, but you can override any of them when creating the `RandomForestClassifier` object.

   ![Training the model](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-fit-model.png)

   *Training the model*

2. Now call the [predict](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier.predict) method to test the model using the values in `test_x`, followed by the [score](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier.score) method to determine the mean accuracy of the model:

   PythonCopy

   ```python
   predicted = model.predict(test_x)
   model.score(test_x, test_y)
   ```

   Confirm that you see the following output:

   ![Testing the model](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-score-model.png)

   *Testing the model*

The mean accuracy is 86%, which seems good on the surface. However, mean accuracy isn't always a reliable indicator of the accuracy of a classification model. Let's dig a little deeper and determine how accurate the model really is — that is, how adept it is at determining whether a flight will arrive on time.

There are several ways to measure the accuracy of a classification model. One of the best overall measures for a binary classification model is [Area Under Receiver Operating Characteristic Curve](https://en.wikipedia.org/wiki/Receiver_operating_characteristic) (sometimes referred to as "ROC AUC"), which essentially quantifies how often the model will make a correct prediction regardless of the outcome. In this unit, you'll compute an ROC AUC score for the model you built previously and learn about some of the reasons why that score is lower than the mean accuracy output by the `score` method. You'll also learn about other ways to gauge the accuracy of the model.

1. Before you compute the ROC AUC, you must generate *prediction probabilities* for the test set. These probabilities are estimates for each of the classes, or answers, the model can predict. For example, `[0.88199435, 0.11800565]`means that there's an 89% chance that a flight will arrive on time (ARR_DEL15 = 0) and a 12% chance that it won't (ARR_DEL15 = 1). The sum of the two probabilities adds up to 100%.

   Run the following code to generate a set of prediction probabilities from the test data:

   PythonCopy

   ```python
   from sklearn.metrics import roc_auc_score
   probabilities = model.predict_proba(test_x)
   ```

2. Now use the following statement to generate an ROC AUC score from the probabilities using scikit-learn's [roc_auc_score](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html) method:

   PythonCopy

   ```python
   roc_auc_score(test_y, probabilities[:, 1])
   ```

   Confirm that the output shows a score of 67%:

   ![Generating an AUC score](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-auc-score.png)

   *Generating an AUC score*

   Why is the AUC score lower than the mean accuracy computed in the previous exercise?

   The output from the `score` method reflects how many of the items in the test set the model predicted correctly. This score is skewed by the fact that the dataset the model was trained and tested with contains many more rows representing on-time arrivals than rows representing late arrivals. Because of this imbalance in the data, you're more likely to be correct if you predict that a flight will be on time than if you predict that a flight will be late.

   ROC AUC takes this into account and provides a more accurate indication of how likely it is that a prediction of on-time *or* late will be correct.

3. You can learn more about the model's behavior by generating a [confusion matrix](https://en.wikipedia.org/wiki/Confusion_matrix), also known as an *error matrix*. The confusion matrix quantifies the number of times each answer was classified correctly or incorrectly. Specifically, it quantifies the number of false positives, false negatives, true positives, and true negatives. This is important, because if a binary classification model trained to recognize cats and dogs is tested with a dataset that is 95% dogs, it could score 95% simply by guessing "dog" every time. But if it failed to identify cats at all, it would be of little value.

   Use the following code to produce a confusion matrix for your model:

   PythonCopy

   ```python
   from sklearn.metrics import confusion_matrix
   confusion_matrix(test_y, predicted)
   ```

   The first row in the output represents flights that were on time. The first column in that row shows how many flights were correctly predicted to be on time, while the second column reveals how many flights were predicted as delayed but weren't. From this, the model appears to be adept at predicting that a flight will be on time.

   ![Generating a confusion matrix](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-confusion-matrix.png)

   *Generating a confusion matrix*

   But look at the second row, which represents flights that were delayed. The first column shows how many delayed flights were incorrectly predicted to be on time. The second column shows how many flights were correctly predicted to be delayed. Clearly, the model isn't nearly as adept at predicting that a flight will be delayed as it is at predicting that a flight will arrive on time. What you *want* in a confusion matrix is large numbers in the upper-left and lower-right corners, and small numbers (preferably zeros) in the upper-right and lower-left corners.

4. Other measures of accuracy for a classification model include *precision* and *recall*. Suppose the model was presented with three on-time arrivals and three delayed arrivals, and that it correctly predicted two of the on-time arrivals, but incorrectly predicted that two of the delayed arrivals would be on time. In this case, the precision would be 50% (two of the four flights it classified as being on time actually were on time), while its recall would be 67% (it correctly identified two of the three on-time arrivals). You can learn more about precision and recall from <https://en.wikipedia.org/wiki/Precision_and_recall>

   Scikit-learn contains a handy method named [precision_score](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html) for computing precision. To quantify the precision of your model, execute the following statements:

   PythonCopy

   ```python
   from sklearn.metrics import precision_score
   
   train_predictions = model.predict(train_x)
   precision_score(train_y, train_predictions)
   ```

   Examine the output. What is your model's precision?

   ![Measuring precision](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-precision.png)

   *Measuring precision*

5. Scikit-learn also contains a method named [recall_score](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html) for computing recall. To measure you model's recall, execute the following statements:

   PythonCopy

   ```python
   from sklearn.metrics import recall_score
   
   recall_score(train_y, train_predictions)
   ```

   What is the model's recall?

   ![Measuring recall](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/3-recall.png)

   *Measuring recall*

6. Use the **File** -> **Save and Checkpoint** command to save the notebook.

In the real world, a trained data scientist would look for ways to make the model even more accurate. Among other things, they would try different algorithms and take steps to *tune* the chosen algorithm to find the optimum combination of parameters. Another likely step would be to expand the dataset to millions of rows rather than a few thousand and also attempt to reduce the imbalance between late and on-time arrivals. But for our purposes, the model is fine as-is.

------

## Next unit: Visualize Output of Model

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-flight-delays-with-python/4-visualize-output)









# Visualize Output of Model

- 8 minutes

In this unit, you'll import Matplotlib into the notebook you've been working with and configure the notebook to support inline Matplotlib output.

1. Switch back to the Azure notebook that you created in the previous section. If you closed the notebook, you can sign back into the [Microsoft Azure Notebooks portal ](https://notebooks.azure.com/), open your notebook, and use the **Cell** -> **Run All** to rerun the all of the cells in the notebook after opening it.

2. Execute the following statements in a new cell at the end of the notebook. Ignore any warning messages that are displayed related to font caching:

   PythonCopy

   ```python
   %matplotlib inline
   import matplotlib.pyplot as plt
   import seaborn as sns
   
   sns.set()
   ```

   The first statement is one of several [magic commands](http://ipython.readthedocs.io/en/stable/interactive/magics.html) supported by the Python kernel that you selected when you created the notebook. It enables Jupyter to render Matplotlib output in a notebook without making repeated calls to [show](https://matplotlib.org/devdocs/api/_as_gen/matplotlib.pyplot.show.html). And it must appear before any references to Matplotlib itself. The final statement configures [Seaborn](https://seaborn.pydata.org/) to enhance the output from Matplotlib.

3. To see Matplotlib at work, execute the following code in a new cell to plot the [ROC curve](https://en.wikipedia.org/wiki/Receiver_operating_characteristic) for the machine-learning model you built in the previous lab:

   PythonCopy

   ```python
   from sklearn.metrics import roc_curve
   
   fpr, tpr, _ = roc_curve(test_y, probabilities[:, 1])
   plt.plot(fpr, tpr)
   plt.plot([0, 1], [0, 1], color='grey', lw=1, linestyle='--')
   plt.xlabel('False Positive Rate')
   plt.ylabel('True Positive Rate')
   ```

4. Confirm that you see the following output:

   ![ROC curve generated with Matplotlib](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/4-roc-curve.png)

   *ROC curve generated with Matplotlib*

The dotted line in the middle of the graph represents a 50-50 chance of obtaining a correct answer. The blue curve represents the accuracy of your model. More importantly, the fact that this chart appears at all demonstrates that you can use Matplotlib in a Jupyter notebook.

The reason you built a machine-learning model is to predict whether a flight will arrive on time or late. In this exercise, you'll write a Python function that calls the machine-learning model you built in the previous lab to compute the likelihood that a flight will be on time. Then you'll use the function to analyze several flights.

1. Enter the following function definition in a new cell, and then run the cell.

   PythonCopy

   ```python
   def predict_delay(departure_date_time, origin, destination):
       from datetime import datetime
   
       try:
           departure_date_time_parsed = datetime.strptime(departure_date_time, '%d/%m/%Y %H:%M:%S')
       except ValueError as e:
           return 'Error parsing date/time - {}'.format(e)
   
       month = departure_date_time_parsed.month
       day = departure_date_time_parsed.day
       day_of_week = departure_date_time_parsed.isoweekday()
       hour = departure_date_time_parsed.hour
   
       origin = origin.upper()
       destination = destination.upper()
   
       input = [{'MONTH': month,
                 'DAY': day,
                 'DAY_OF_WEEK': day_of_week,
                 'CRS_DEP_TIME': hour,
                 'ORIGIN_ATL': 1 if origin == 'ATL' else 0,
                 'ORIGIN_DTW': 1 if origin == 'DTW' else 0,
                 'ORIGIN_JFK': 1 if origin == 'JFK' else 0,
                 'ORIGIN_MSP': 1 if origin == 'MSP' else 0,
                 'ORIGIN_SEA': 1 if origin == 'SEA' else 0,
                 'DEST_ATL': 1 if destination == 'ATL' else 0,
                 'DEST_DTW': 1 if destination == 'DTW' else 0,
                 'DEST_JFK': 1 if destination == 'JFK' else 0,
                 'DEST_MSP': 1 if destination == 'MSP' else 0,
                 'DEST_SEA': 1 if destination == 'SEA' else 0 }]
   
       return model.predict_proba(pd.DataFrame(input))[0][0]
   ```

   This function takes as input a date and time, an origin airport code, and a destination airport code, and returns a value between 0.0 and 1.0 indicating the probability that the flight will arrive at its destination on time. It uses the machine-learning model you built in the previous lab to compute the probability. And to call the model, it passes a DataFrame containing the input values to `predict_proba`. The structure of the DataFrame exactly matches the structure of the DataFrame we used earlier.

    Note

   Date input to the `predict_delay` function use the international date format `dd/mm/year`.

2. Use the code below to compute the probability that a flight from New York to Atlanta on the evening of October 1 will arrive on time. The year you enter is irrelevant because it isn't used by the model.

   PythonCopy

   ```python
   predict_delay('1/10/2018 21:45:00', 'JFK', 'ATL')
   ```

   Confirm that the output shows that the likelihood of an on-time arrival is 60%:

   ![Predicting whether a flight will arrive on time](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/4-jfk-to-atl.png)

   *Predicting whether a flight will arrive on time*

3. Modify the code to compute the probability that the same flight a day later will arrive on time:

   PythonCopy

   ```python
   predict_delay('2/10/2018 21:45:00', 'JFK', 'ATL')
   ```

   How likely is this flight to arrive on time? If your travel plans were flexible, would you consider postponing your trip for one day?

4. Now modify the code to compute the probability that a morning flight the same day from Atlanta to Seattle will arrive on time:

   PythonCopy

   ```python
   predict_delay('2/10/2018 10:00:00', 'ATL', 'SEA')
   ```

   Is this flight likely to arrive on time?

You now have an easy way to predict, with a single line of code, whether a flight is likely to be on time or late. Feel free to experiment with other dates, times, origins, and destinations. But keep in mind that the results are only meaningful for the airport codes ATL, DTW, JFK, MSP, and SEA because those are the only airport codes the model was trained with.

1. Execute the following code to plot the probability of on-time arrivals for an evening flight from JFK to ATL over a range of days:

   PythonCopy

   ```python
   import numpy as np
   
   labels = ('Oct 1', 'Oct 2', 'Oct 3', 'Oct 4', 'Oct 5', 'Oct 6', 'Oct 7')
   values = (predict_delay('1/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('2/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('3/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('4/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('5/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('6/10/2018 21:45:00', 'JFK', 'ATL'),
             predict_delay('7/10/2018 21:45:00', 'JFK', 'ATL'))
   alabels = np.arange(len(labels))
   
   plt.bar(alabels, values, align='center', alpha=0.5)
   plt.xticks(alabels, labels)
   plt.ylabel('Probability of On-Time Arrival')
   plt.ylim((0.0, 1.0))
   ```

2. Confirm that the output looks like this:

   ![Probability of on-time arrivals for a range of dates](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/4-predict-plot-1.png)

   *Probability of on-time arrivals for a range of dates*

3. Modify the code to produce a similar chart for flights leaving JFK for MSP at 1:00 p.m. on April 10 through April 16. How does the output compare to the output in the previous step?

4. On your own, write code to graph the probability that flights leaving SEA for ATL at 9:00 a.m., noon, 3:00 p.m., 6:00 p.m., and 9:00 p.m. on January 30 will arrive on time. Confirm that the output matches this:

   ![Probability of on-time arrivals for a range of times](https://docs.microsoft.com/en-us/learn/student-evangelism/predict-flight-delays-with-python/media/4-predict-plot-2.png)

   *Probability of on-time arrivals for a range of times*

If you are new to Matplotlib and would like to learn more about it, you will find an excellent tutorial at [https://www.labri.fr/perso/nrougier/teaching/matplotlib/.](https://www.labri.fr/perso/nrougier/teaching/matplotlib/) There is *much* more to Matplotlib than what was shown here, which is one reason why it is so popular in the Python community.

------

## Next unit: Summary and knowledge check

[Continue](https://docs.microsoft.com/en-us/learn/modules/predict-flight-delays-with-python/5-summary)











# Summary and knowledge check

- 5 minutes

In this module, you learned how to:

- Create a notebook in Azure Notebooks
- Import data into a notebook using `curl`
- Use [Pandas](https://pandas.pydata.org/pandas-docs/stable/) to clean and prepare data
- Use [scikit-learn](http://scikit-learn.org/stable/) to build a machine-learning model
- Use [Matplotlib](https://matplotlib.org/) to visualize the results

Pandas, scikit-learn, and Matplotlib are among the most popular Python libraries on the planet. With them, you can prepare data for use in machine learning, build sophisticated machine-learning models from the data, and chart the output. Jupyter notebooks provide a ready-made environment for using these libraries, and Azure Notebooks give you easy access to Jupyter notebooks without requiring you to install any software or set up a Jupyter environment on a server.

## Check your knowledge

\1. 

What method is used in Pandas to import a CSV file? Assume pandas was loaded as `import pandas as pd`.



pd.load_file('file.csv')



pd.read_file('file.csv')



pd.read_csv('file.csv')

\2. 

What is the purpose of splitting data before training a machine learning model?



To not give the model too much data.



One part can be used for training and the other can be used to evaluate the model's performance.



The model doesn't need much data.

\3. 

Assuming you've imported Matplotlib as 'plt', what is the method on Matplotlib that you would use to plot a bar chart?



plt.bar(labels, values)



plt.chart(labels, values)



plt.barchart(labels, values)









# PART 3: Analyze the sentiment of reviews with Keras



# Introduction

- 5 minutes

Building neural networks isn't easy. Even with popular libraries such as the [Microsoft Cognitive Toolkit](https://www.microsoft.com/cognitive-toolkit/) and [TensorFlow](https://www.tensorflow.org/) to help out, it often requires several hundred lines of code to get a neural network up and running. That's one reason [Keras](https://keras.io/)has become popular in the deep-learning community. Keras is an open-source Python library that dramatically simplifies the building of neural networks. Under the hood, it uses the Microsoft Cognitive Toolkit, TensorFlow, or [Theano](https://github.com/Theano) to do the heavy lifting. With Keras, you can build sophisticated neural networks with just a few dozen lines of code and train them to classify images, analyze text for sentiment, do natural-language processing, and perform other tasks at which deep learning excels.

![Keras documentation](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/0-keras.png)

In this module, you'll use Keras to build a neural network that scores text for sentiment. An input such as "Great service, and some of the best sushi I've ever tasted" will score close to 1.0 indicating the sentiment is positive, while an input such as "The food was bland and the service was terrible" will score closer to 0.0. Such systems are widely used today to monitor Twitter, Yelp, and other social-media services for sentiment regarding businesses and political candidates. To minimize setup and configuration, you'll use Keras in a [Jupyter notebook](http://jupyter.org/) hosted in [Azure Notebooks](https://notebooks.azure.com/), where Keras, TensorFlow, and other libraries that you need are preinstalled.

## Learning objectives

In this module, you will:

- Create a Jupyter notebook in Azure Notebooks
- Use Keras to build and train a neural network to perform sentiment analysis
- Use the neural network to analyze text for sentiment

------

## Next unit: Create an Azure Notebook

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-review-sentiment-with-keras/1-create-an-azure-notebook)


  



# Create an Azure Notebook

- 10 minutes

The first order of business is to create a new Azure notebook. Azure notebooks are contained in *projects* whose primary purpose is to group related notebooks. In this unit, you'll create a new project and then create a notebook inside it.

1. Navigate to [https://notebooks.azure.com ](https://notebooks.azure.com/) in your browser.

2. Sign in using your Microsoft account.

3. Click **My Projects**.

   ![Navigating to the Projects page](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/1-add-project-1.png)

   *Navigating to the Projects page*

4. Click **+ New Project**. Then create a new project named "Keras". You may uncheck the "Public project" box if you'd like, but making the library public allows the notebooks in it to be shared with others through links, social media, or e-mail. If you're unsure which to choose, you can easily change a notebook to public or private later on.

   ![Creating a project](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/1-add-project-2.png)

   *Creating a project*

5. Click the **+** sign to add a notebook to the project.

   ![Adding a notebook to the project](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/1-add-notebook-1.png)

   *Adding a notebook to the project*

6. Name the notebook "kerasnotebook.ipynb" and select **Python 3.6 Notebook** as the item type. This will create a notebook with a Python 3.6 kernel. One of the strengths of Jupyter notebooks is that you can use different languages by choosing different kernels.

   ![Creating a notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/1-add-notebook-2.png)

   *Creating a notebook*

   If you're curious, the **.ipynb** file-name extension stands for "IPython notebook." Jupyter notebooks were originally known as IPython (Interactive Python) notebooks, and they only supported Python as a programming language. The name Jupyter is a combination of Julia, Python, and R — the core programming languages that Jupyter supports.

7. Click the new notebook. This will launch the notebook and allow you to start editing it.

   ![Opening the notebook](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/1-open-notebook.png)

   *Opening the notebook*

You can create additional projects and notebooks as you work with Azure Notebooks. You can create notebooks from scratch, or you can upload existing notebooks. In the next exercise, you will use the notebook you created to build a neural network from scratch.

------

## Next unit: Build and Train a Neural Network

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-review-sentiment-with-keras/2-build-and-train-a-neural-network)


  





# Build and Train a Neural Network

- 5 minutes

In this unit, you'll use Keras to build and train a neural network that analyzes text for sentiment. In order to train a neural network, you need data to train it with. Rather than download an external dataset, you'll use the [IMDB movie reviews sentiment classification](https://keras.io/datasets/#imdb-movie-reviews-sentiment-classification) dataset that's included with Keras. The IMDB dataset contains 50,000 movie reviews that have been individually scored as positive (1) or negative (0). The dataset is divided into 25,000 reviews for training and 25,000 reviews for testing. The sentiment that's expressed in these reviews is the basis for which your neural network will analyze text presented to it and score it for sentiment.

> The IMDB dataset is one of several useful datasets included with Keras. For a complete list of built-in datasets, see [https://keras.io/datasets/.](https://keras.io/datasets/)

1. Type or paste the following code into the notebook's first cell and click the **Run** button (or press **Shift+Enter**) to execute it and add a new cell below it:

   PythonCopy

   ```python
   from keras.datasets import imdb
   top_words = 10000
   (x_train, y_train), (x_test, y_test) = imdb.load_data(num_words=top_words)
   ```

   This code loads the IMDB dataset that's included with Keras and creates a dictionary mapping the words in all 50,000 reviews to integers indicating the words' relative frequency of occurrence. Each word is assigned a unique integer. The most common word is assigned the number 1, the second most common word is assigned the number 2, and so on. `load_data` also returns a pair of tuples containing the movie reviews (in this example, `x_train` and `x_test`) and the 1s and 0s classifying those reviews as positive and negative (`y_train` and `y_test`).

2. Confirm that you see the message "Using TensorFlow backend" indicating that Keras is using TensorFlow as its back end.

   ![Loading the IMDB dataset](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-using-tensorflow.png)

   *Loading the IMDB dataset*

   If you wanted Keras to use the Microsoft Cognitive Toolkit, also known as CNTK, as its back end, you could do so by adding a few lines of code at the beginning of the notebook. For an example, see [CNTK and Keras in Azure Notebooks](http://www.johndehavilland.com/blog/2017/12/19/keras-and-cntk-azure-notebooks.html).

3. So what exactly did the `load_data` function load? The variable named `x_train` is a list of 25,000 lists, each of which represents one movie review. (`x_test` is also a list of 25,000 lists representing 25,000 reviews. `x_train` will be used for training, while `x_test` will be used for testing.) But the inner lists — the ones representing movie reviews — don't contain words; they contain integers. Here's how it's described in the Keras documentation:

   ![Keras documentation](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-keras-docs.png)

   The reason the inner lists contain numbers rather than text is that you don't train a neural network with text; you train it with numbers. Specifically, you train it with [tensors](https://en.wikipedia.org/wiki/Tensor). In this case, each review is a 1-dimensional tensor (think of a 1-dimensional array) containing integers identifying the words contained in the review. To demonstrate, type the following Python statement into an empty cell and execute it to see the integers representing the first review in the training set:

   PythonCopy

   ```python
   x_train[0]
   ```

   ![Integers comprising the first review in the IMDB training set](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-review-indices.png)

   *Integers comprising the first review in the IMDB training set*

   The first number in the list — 1 — doesn't represent a word at all. It marks the start of the review and is the same for every review in the dataset. The numbers 0 and 2 are reserved as well, and you subtract 3 from the other numbers to map an integer in a review to the corresponding integer in the dictionary. The second number — 14 — references the word that corresponds to the number 11 in the dictionary, the third number represents the word assigned the number 19 in the dictionary, and so on.

4. Curious to see what the dictionary looks like? Execute the following statement in a new notebook cell:

   PythonCopy

   ```python
   imdb.get_word_index()
   ```

   Only a subset of the dictionary entries is shown, but in all, the dictionary contains more than 88,000 words and the integers that correspond to them. The output you see will probably not match the output in the screenshot because the dictionary is generated anew each time `load_data` is called.

   ![Dictionary mapping words to integers](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-word-index.png)

   *Dictionary mapping words to integers*

5. As you have seen, each review in the dataset is encoded as a collection of integers rather than words. Is it possible to reverse-encode a review so you can see the original text that comprised it? Enter the following statements into a new cell and execute them to show the first review in `x_train` in textual format:

   PythonCopy

   ```python
   word_dict = imdb.get_word_index()
   word_dict = { key:(value + 3) for key, value in word_dict.items() }
   word_dict[''] = 0  # Padding
   word_dict['>'] = 1 # Start
   word_dict['?'] = 2 # Unknown word
   reverse_word_dict = { value:key for key, value in word_dict.items() }
   print(' '.join(reverse_word_dict[id] for id in x_train[0]))
   ```

   In the output, ">" marks the beginning of the review, while "?" marks words that aren't among the most common 10,000 words in the dataset. These "unknown" words are represented by 2s in the list of integers representing a review. Remember the `num_words` parameter you passed to `load_data`? This is where it comes into play. It doesn't reduce the size of the dictionary, but it restricts the range of integers used to encode the reviews.

   ![The first review in textual format](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-review-text.png)

   *The first review in textual format*

6. The reviews are "clean" in the sense that letters have been converted to lowercase and punctuation characters removed. But they are not ready to train a neural network to analyze text for sentiment. When you train a neural network with collection of tensors, each tensor needs to be the same length. At present, the lists representing reviews in `x_train` and `x_test` have varying lengths.

   Fortunately, Keras includes a function that takes a list of lists as input and converts the inner lists to a specified length by truncating them if necessary or padding them with 0s. Enter the following code into the notebook and run it to force all the lists representing movie reviews in `x_train` and `x_test` to a length of 500 integers:

   PythonCopy

   ```python
   from keras.preprocessing import sequence
   max_review_length = 500
   x_train = sequence.pad_sequences(x_train, maxlen=max_review_length)
   x_test = sequence.pad_sequences(x_test, maxlen=max_review_length)
   ```

7. Now that the training and testing data is prepared, it is time to build the model! Run the following code in the notebook to create a neural network that performs sentiment analysis:

   PythonCopy

   ```python
   from keras.models import Sequential
   from keras.layers import Dense
   from keras.layers.embeddings import Embedding
   from keras.layers import Flatten
   
   embedding_vector_length = 32
   model = Sequential()
   model.add(Embedding(top_words, embedding_vector_length, input_length=max_review_length))
   model.add(Flatten())
   model.add(Dense(16, activation='relu'))
   model.add(Dense(16, activation='relu'))
   model.add(Dense(1, activation='sigmoid'))
   model.compile(loss='binary_crossentropy',optimizer='adam', metrics=['accuracy'])
   print(model.summary())
   ```

   Confirm that the output looks like this:

   ![Creating a neural network with Keras](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-build-model.png)

   *Creating a neural network with Keras*

   This code is the essence of how you construct a neural network with Keras. It first instantiates a `Sequential` object representing a "sequential" model — one that is composed of an end-to-end stack of layers in which the output from one layer provides input to the next.

   The next several statements add layers to the model. First is an [embedding layer](https://keras.io/layers/embeddings/), which is crucial to neural networks that process words. The embedding layer essentially maps many-dimensional arrays containing integer word indexes into floating-point arrays containing fewer dimensions. It also allows words with similar meanings to be treated alike. A full treatment of word embeddings is beyond the scope of this lab, but you can learn more by reading [Why You Need to Start Using Embedding Layers](https://towardsdatascience.com/deep-learning-4-embedding-layers-f9a02d55ac12). If you prefer a more scholarly explanation, refer to [Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/pdf/1301.3781.pdf). The call to [Flatten](https://keras.io/layers/core/#flatten) following the addition of the embedding layer reshapes the output for input to the next layer.

   The next three layers added to the model are [dense](https://keras.io/layers/core/#dense) layers, also known as *fully connected* layers. These are the traditional layers that are common in neural networks. Each layer contains *n* nodes or [neurons](https://en.wikipedia.org/wiki/Artificial_neuron), and each neuron receives input from every neuron in the previous layer, hence the term "fully connected." It is these layers that permit a neural network to "learn" from input data by iteratively guessing at the output, checking the results, and fine-tuning the connections to produce better results. The first two dense layers in this network contain 16 neurons each. This number was arbitrarily chosen; you might be able to improve the accuracy of the model by experimenting with different sizes. The final dense layer contains just one neuron because the ultimate goal of the network is to predict one output — namely, a sentiment score from 0.0 to 1.0.

   The result is the neural network pictured below. The network contains an input layer, an output layer, and two hidden layers (the dense layers containing 16 neurons each). For comparison, some of today's more sophisticated neural networks have more than 100 layers. One example is [ResNet-152](https://blogs.microsoft.com/ai/microsoft-researchers-win-imagenet-computer-vision-challenge/) from Microsoft Research, whose accuracy at identifying objects in photographs sometimes exceeds that of a human. You could build ResNet-152 with Keras, but you would need a cluster of GPU-equipped computers to train it from scratch.

   ![Visualizing the neural network](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-neural-network.png)

   *Visualizing the neural network*

   The call to the [compile](https://keras.io/models/model/#compile) function "compiles" the model by specifying important parameters such as which [optimizer](https://keras.io/optimizers/)to use and what [metrics](https://keras.io/metrics/) to use to judge the accuracy of the model in each training step. Training doesn't begin until you call the model's `fit` function, so the `compile` call typically executes quickly.

8. Now call the [fit](https://keras.io/models/model/#fit) function to train the neural network:

   PythonCopy

   ```python
   hist = model.fit(x_train, y_train, validation_data=(x_test, y_test), epochs=5, batch_size=128)
   ```

   Training should take about 6 minutes, or a little more than 1 minute per epoch. `epochs=5` tells Keras to make 5 forward and backward passes through the model. With each pass, the model learns from the training data and measures ("validates") how well it learned using the test data. Then it makes adjustments and goes back for the next pass or *epoch*. This is reflected in the output from the `fit` function, which shows the training accuracy (`acc`) and validation accuracy (`val_acc`) for each epoch.

   `batch_size=128` tells Keras to use 128 training samples at a time to train the network. Larger batch sizes speed the training time (fewer passes are required in each epoch to consume all of the training data), but smaller batch sizes sometimes increase accuracy. Once you've completed this lab, you might want to go back and retrain the model with a batch size of 32 to see what effect, if any, it has on the model's accuracy. It roughly doubles the training time.

   ![Training the model](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-train-model.png)

   *Training the model*

9. This model is unusual in that it learns well with just a few epochs. The training accuracy quickly zooms to near 100%, while the validation accuracy goes up for an epoch or two and then flattens out. You generally don't want to train a model for any longer than is required for these accuracies to stabilize. The risk is [overfitting](https://en.wikipedia.org/wiki/Overfitting), which results in the model performing well against test data but not so well with real-world data. One indication that a model is overfitting is a growing discrepancy between the training accuracy and the validation accuracy. For a great introduction to overfitting, see [Overfitting in Machine Learning: What It Is and How to Prevent It](https://elitedatascience.com/overfitting-in-machine-learning).

   To visualize the changes in training and validation accuracy as training progress, execute the following statements in a new notebook cell:

   PythonCopy

   ```python
   import seaborn as sns
   import matplotlib.pyplot as plt
   %matplotlib inline
   
   sns.set()
   acc = hist.history['acc']
   val = hist.history['val_acc']
   epochs = range(1, len(acc) + 1)
   
   plt.plot(epochs, acc, '-', label='Training accuracy')
   plt.plot(epochs, val, ':', label='Validation accuracy')
   plt.title('Training and Validation Accuracy')
   plt.xlabel('Epoch')
   plt.ylabel('Accuracy')
   plt.legend(loc='upper left')
   plt.plot()
   ```

   The accuracy data comes from the `history` object returned by the model's `fit` function. Based on the chart that you see, would you recommend increasing the number of training epochs, decreasing it, or leaving it the same?

10. Another way to check for overfitting is to compare training loss to validation loss as training proceeds. Optimization problems such as this seek to minimize a loss function. You can read more [here](https://en.wikipedia.org/wiki/Loss_function). For a given epoch, training loss, much greater than validation loss, can be evidence of overfitting. In the previous step, you used the `acc` and `val_acc` properties of the `history` object's `history` property to plot training and validation accuracy. The same property also contains values named `loss` and `val_loss` representing training and validation loss, respectively. If you wanted to plot these values to produce a chart like the one below, how would you modify the code above to do it?

    ![Training and validation loss](https://docs.microsoft.com/en-us/learn/student-evangelism/analyze-review-sentiment-with-keras/media/2-loss-chart.png)

    *Training and validation loss*

    Given that the gap between training and validation loss begins increasing in the third epoch, what would you say if someone suggested that you increase the number of epochs to 10 or 20?

11. Finish up by calling the model's `evaluate` method to determine how accurately the model is able to quantify the sentiment expressed in text based on the test data in `x_test` (reviews) and `y_test` (0s and 1s, or "labels," indicating which reviews are positive and which are negative):

    PythonCopy

    ```python
    scores = model.evaluate(x_test, y_test, verbose=0)
    print("Accuracy: %.2f%%" % (scores[1] * 100))
    ```

    What is the computed accuracy of your model?

You probably achieved an accuracy in the 85% to 90% range. That's acceptable considering you built the model from scratch (as opposed to using a pretrained neural network) and the training time was short even without a GPU. It *is*possible to achieve accuracies of 95% or higher with alternate neural network architectures, particularly [recurrent neural networks](https://en.wikipedia.org/wiki/Recurrent_neural_network) (RNNs) that utilize [Long Short-Term Memory](https://en.wikipedia.org/wiki/Long_short-term_memory) (LSTM) layers. Keras makes it easy to build such networks, but training time can increase exponentially. The model that you built strikes a reasonable balance between accuracy and training time. However, if you would like to learn more about building RNNs with Keras, see [Understanding LSTM and its Quick Implementation in Keras for Sentiment Analysis](https://towardsdatascience.com/understanding-lstm-and-its-quick-implementation-in-keras-for-sentiment-analysis-af410fd85b47).

## Check your knowledge

\1. 

Based on the first chart you created ('Training and Validation Accuracy'), would you recommend increasing the number of training epochs, decreasing it, or leaving it the same?



Increasing the number of training epochs



Decreasing the number of training epochs.



Leaving 5 training epochs









# Use the Neural Network to Analyze Text for Sentiment

- 5 minutes

The real test comes when you input text of your own into the model and see how it performs — that is, how adept it is at quantifying the sentiment expressed in that text. In this unit, you'll write a Python function that accepts a text string as input, passes it to the model, and returns a sentiment score. Then you'll use the function to analyze the sentiment expressed in various text strings.

1. Add the following code to a cell at the end of the notebook and run the cell:

   PythonCopy

   ```python
   import string
   import numpy as np
   
   def analyze(text):
       # Prepare the input by removing punctuation characters, converting
       # characters to lower case, and removing words containing numbers
       translator = str.maketrans('', '', string.punctuation)
       text = text.translate(translator)
       text = text.lower().split(' ')
       text = [word for word in text if word.isalpha()]
   
       # Generate an input tensor
       input = [1]
       for word in text:
           if word in word_dict and word_dict[word] < top_words:
               input.append(word_dict[word])
           else:
               input.append(2)
       padded_input = sequence.pad_sequences([input], maxlen=max_review_length)
   
       # Invoke the model and return the result
       result = model.predict(np.array([padded_input][0]))[0][0]
       return result
   ```

   These statements define a function named `analyze` that accepts a string as input and returns a number from 0.0 to 1.0 quantifying the sentiment expressed in that string. The higher the number, the more positive the sentiment. The function cleans the input string, converts it into a list of integers referencing words in the dictionary created by the `load_data` function, and finally calls the model's `predict` function to score the text for sentiment.

2. Use the notebook to execute the following statement:

   PythonCopy

   ```python
   analyze('Easily the most stellar experience I have ever had.')
   ```

   The output is the sentiment expressed in the input text as a number from 0.0 to 1.0. Would you agree with the model's assessment?

3. Now try this statement:

   PythonCopy

   ```python
   analyze('The long lines and poor customer service really turned me off.')
   ```

   How does the model quantify the sentiment expressed in this text?

Finish up by testing the model with input strings of your own. The results won't be perfect, but you should find that the model is reasonably adept at quantifying sentiment. Even though the model was trained with movie reviews, it isn't *limited*to analyzing movie reviews. That makes sense because there are inherent similarities between language expressing the like or dislike of a movie and words expressing feelings about other unrelated subjects.

------

## Next unit: Summary and knowledge check

[Continue](https://docs.microsoft.com/en-us/learn/modules/analyze-review-sentiment-with-keras/4-summary)







# Summary and knowledge check

- 10 minutes

Keras makes it remarkably easy to build and train neural networks to perform a wide range of deep-learning tasks. It doesn't absolve you from understanding various neural network architectures, knowing what types of layers to include in a network or the sizes of those layers, or, for example, understanding the role of activation functions and when to apply activation functions of different types, but once you've determined what to build, a few lines of code generally gets the job done. Moreover, Keras allows you to experiment with different network architectures and implementations and rather quickly compare the results.

## Learn more

If you would like to learn more about Keras, there are some great online resources available, including the [Keras blog](https://blog.keras.io/). You may also want to follow [François Chollet](https://twitter.com/fchollet) on Twitter. François is the author of Keras as well as the author of the book [Deep Learning with Python](https://www.amazon.com/Deep-Learning-Python-Francois-Chollet/dp/1617294438), which is the ultimate self-learning guide for Keras. In addition to introducing Keras and providing key insights to help you use it effectively, the book provides a working introduction to deep learning that is independent of the platforms and libraries that you use.

## Check your knowledge

\1. 

What best describes Keras?



It is a deep learning library to build neural networks.



It is a library to help clean data.



It is an API wrapper on top of deep learning libraries such as TensorFlow and the Microsoft Cognitive Toolkit.

\2. 

What does calling `model.summary()` do?



Produces a summary of layers for the compiled model.



Produces a summary of the training data used in the model.



Produces a summary of the predictions made from the model.

\3. 

What method on the model is used to make a prediction on new data?



evaluate



predict



forecast



