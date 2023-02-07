# Taxi trips example

Simulating real traffic using the [*New York City Taxi Trip Duration* dataset](https://www.kaggle.com/c/nyc-taxi-trip-duration) 🚕

First of all you need a running instance of Beaver. For instance, you can to the root of this repo and start an instance in the background:

```sh
(cd ... && docker-compose up -d)
```

Beaver is being run in a Docker container. You'll interact with it from your host machine. You need to install some Python dependencies to do that. We'll install them in a virtual environment 🐍

```sh
venv .venv
source .venv/bin/activate
pip install -r requirements.txt

```

If notebook does not start in newly created venv then do the following.
Create kernel and start the notebook after.
(Note: if running pyenv, need to deactivate that first)

```sh
ipython kernel install --user --name=venv
jupyter notebook
```

After notebook has started, make sure that selected kernel is `venv`

Now we can simulate traffic. The order is the same as what happened in production. This is because we know the departure and arrival times of each taxi trip, and can thus reproduce the exact same timeline. We'll apply a x15 speed-up to make things more exciting ⚡️

```sh
python simulate.py --speed 15
```


Now [`tutorial.ipynb`](tutorial.ipynb) and follow the steps therein 👋
