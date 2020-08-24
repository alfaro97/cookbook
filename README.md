### Database collections example

**Sample User doc**
```
“_id”: 5ba6a0cfd4cff52894ef222a
“username”: "admin"
“Firstname”: "Joe"
“lastname”: "Bloggs"
“hashed_password”: "sha256$d9uQWVAk$f2b4bddfc8d858ed7842d8c93813b426036da4451c7a5419f8688e..."
“recipe_votes”: 
[
     5ba6a0cfd4cff52894efefkv,
     5ba6a0cfd4cff52894ejijnie
]
```




### IDE - SETUP - VSCODE

1.	After opening vscode I created a workspace
2.	Create ‘venv’ directory for virtual environment. Bash terminal: py -3 -m venv venv
3.	Open the project folder
4.	View – Command Palette
5.	Python: Select Interpreter
6.	Python: Create Terminal
7.	Install flask in that virtual env:  pip3 install flask
8.	Upgrade pip: python -m pip install --upgrade pip
9.	Debug - Open Configurations-Python
```
{
            "name": "Python: Flask (development mode)",
            "type": "python",
            "request": "launch",
            "module": "flask",
            "env": {
                "FLASK_APP": "app.py",
                "FLASK_ENV": "development"
            },
            "args": [
                "run"
            ]
}
```




### IDE - SETUP - MongoDB

1.	mLab: Create new database – cookbook
2.	Later in the project during development, I created a local mongodb database
3.	To connect using the mongo shell:
`mongo ds251332.mlab.com:51332/cookbook -u <dbuser> -p <dbpassword>
mongodb://localhost:27017/cookbook`
4.	To connect using a driver via the standard MongoDB URI
`mongodb://<dbuser>:<dbpassword>@ds251332.mlab.com:51332/cookbook`
5.	pip3 install flask_pymongo



### IDE - SETUP - Other installations and setup

*   **iPython**:	pip3 install ipython
*   **jupyter***:	pip3 install jupyter
*   **matplotlib**:	pip3 install matplotlib
*   **pandas**:	pip3 install pandas
*   **PyLint install**:	pip install -U pylint

*   **Run jupyter**:	jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser
*   **Create requirements.txt**:	pip3 freeze --local > requirements.txt
*   **Create Procfile**:	echo web: python app.py > Procfile


