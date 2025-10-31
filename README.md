# InfoCom Drone Project - Part 1 - Drone simulation on Raspberry Pi
Install the required Python packages if not done already (some packages might already be installed):
```
sudo apt update
sudo apt install python3-socketio
sudo apt install python3-engineio
sudo apt install python3-flask-socketio
sudo apt install python3-flask-cors

```
Go to the `webserver` folder in a terminal window, run the flask server:
```
export FLASK_APP=build.py
export FLASK_DEBUG=1
flask run
```
Go to the `pi` folder in another terminal window, run the Pi controller:
```
python3 pi_controller.py
```
Open a web browser, e.g. Chromium, and go to `http://localhost:5000`.

In the terminal running `pi_controller.py`, use the keys 'wasd' to move the 'drone' on the website. 

Note: Don't use `python3 build.py` to run the webserver, since this does not porvide all the functionalities required by the application.

