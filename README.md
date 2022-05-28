# Duke-ids_706-Data-Engineering-System
#duke-data-engineering
# Cousera Course 1: Python and Pandas for Data Engineering
## Week 1
### Install vs. Unintall packages
  - `python -m pip --version` - check version
  - `pip install pytest`-install the packages
  - `pip list` - check all the installed packages
  - `pip help` - get all the commands in pip
  - `pip install pytest==6.2.2` - install specific version of the package
  - `pip install pytest -- upgrade` - upgrade the package to the newest version
### Saving Requirements File in Python
- Shell commends
- ls: list the commands of a directory
- cat: prints the conent of a file to the screen
- `pip freeze > requirements.txt`- create a requirements file with the packages installed using pip
### Create a Virtual Environment
- `python -m venv ~/envs/...` : To create a virtual environment named '...'
- `source ~/envs/.../bin/activate`:activate new environment
- `pip list`: To see the packages installed in your environment.
- `pip install -r requirements.txt` : install the packages saved to your requirements file from the previous lab.
- `deactivate`: deactivate the environment

## Week 2
### 3 ways creating dictionaries
- dict(Name= 'bella'    , Age=  21 )
- data = [['Name',  'bella'   ], ['Age',   21]]
dict(data)
- {'Name':  'bella'    , 'Age': 21  }
### creating fibonacci series by using generators
![alt text](img width="361" alt="Screen Shot 2022-05-23 at 1 11 49 AM" src="https://user-images.githubusercontent.com/60382493/169774354-706f5719-8b25-47b0-938e-2c6d516c4aee.png")

### Comprehension using curly brackets will produce a dictionary. 
- `name = 'bella'`
- `items = zip(list(name), list(range(len(name))))`
- `print(items)`
- `{x:y for x,y in items}`
  
## Week 3
### Creating NumPy Arrays in Python
- ndarray: multi-dimensional data, single data type, complex numerical calculations
- dataframe: 2d data,multiple data types, data analysis, data visualization
### Spark and PySpark DataFrames in Python
- Hadoop and Spark both distributed, allow scale horizontally
- Spark: distirbuted Dataframes using java virtual machine (JVM)
- Lazy evaluation: operations stacked behind scenes, results not calculated immediately
- pandas uses eager evaluation: get an output then run the following, very interactive and easy to debug
- Spark: good for big data, like csv > 1GB,  debug is challenging, great for making transformations in big data
## Creating Dask DataFrames in Python
- distributed operations
- wraps pandas df and np arrays
- `import dask.dataframe as dd`, can use the function `dd.from_pandas(df, n_partitions = 3)`
- didn't give the exact data and results as output, because it uses the lazy evaluation
- `ddf.std().compute()` will give the result, but`ddf.std()` will not; need to call `compute()`
- call `result.dask`  and `result.visualize()` will generate graph for visalization
- Big data: choose PySpark or Dask
- choose between PySpark or Dask: based on ur enterprise: PySpark documentation goood good, maturity of product; Dask is python natives, can use pandas and numpy full capabilities, dask good if u know ur pipelines
## Week 4
### Vim Normal Mode
- Some mode in terminal: 
- h - move left
- j - move down
- k - move up
- l - move right
