# Map-Game

Installation instructions
Create a text file named "requirements.txt"
Paste the following:

click==7.1.2

Flask==1.1.2

itsdangerous==1.1.0

Jinja2==2.11.2

kaleido==0.0.3.post1

MarkupSafe==1.1.1

numpy==1.19.4

pandas==1.1.4

pkg-resources==0.0.0

plotly==4.13.0

python-dateutil==2.8.1

pytz==2020.4

retrying==1.3.3

six==1.15.0

Werkzeug==1.0.1

Launch your local version of linux (wsl, ubuntu)
Ubuntu 18.04+ should come with both Python 2 and Python 3 installed. Double check with:
python3 -V
You should receive output of the python version.
Next, make sure you have pip3 with:
pip3 -V
If you don't have it, run:
sudo apt-get install python3-pip

Next, we want to use the virtual environment setup for Python:
sudo apt install -y python3-venv

Make a directory for your environments and then create the environment "map-game":
mkdir environments
cd environments
python3 -m venv map-game

To launch the environment, run:
source map-game/bin/activate

To download dependencies, run:
pip3 install -r requirements.txt

The virtual Python 3 environment is now set up with Flask and the dependencies needed to run the software.

Next, you want to copy over the app.py, static (folder), and templates (folder) to the map-game directory.
Finally, run the following lines to ensure that the environment variables are set properly for development:
export FLASK_APP=app
export FLASK_ENV=development

After this, you should be good to launch the development build!
python -m flask run








