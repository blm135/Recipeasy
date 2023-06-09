# Recipeasy

## To run the frontend

1. cd into my-app
2. run `npm start`

Note...
If you get an error like this:
> my-app@0.1.0 start
> react-scripts start
'react-scripts' is not recognized as an internal or external command,
operable program or batch file.

... run `npm install` and it should fix it

## To run the backend

1. In `recipeasy/my-app/l` create a python virtual environment
   1. [You can find more here](https://flask.palletsprojects.com/en/2.2.x/installation/) in the virtual environment section
python3 -m venv venv
. venv/bin/activate

2. Activate your virtual environment
3. Run `pip install flask`
4. Run `pip install flask-jwt-extended`
5. Run ` pip install flask_sqlalchemy`
6. Run `pip install flask-cors`
7. Then run your backend by running `flask --app base.py run` while in the `/backend` folder.

## To initialize local database

1. Run the command `flask --app base.py initdb` after you've already setup your virtual environment
2. Run the command `flask --app base.py filldb` after you've already setup your virtual environment, this populates the ingredients dropdown

## To test login and authorization

1. Make sure your token is updated
2. /profile will tell you if you are authorized or not
3. username: test password: test
4. This will be overhauled and it is just a temporary solution while we get the database and further logic scaled up.
