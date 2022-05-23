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
![alt text](<img width="361" alt="Screen Shot 2022-05-23 at 1 11 49 AM" src="https://user-images.githubusercontent.com/60382493/169774254-02124014-1df5-4ea0-a57b-3489fcf7054c.png">)

### Comprehension using curly brackets will produce a dictionary. 
- `name = 'bella'`
- `items = zip(list(name), list(range(len(name))))`
- `print(items)`
- `{x:y for x,y in items}`
  
  
