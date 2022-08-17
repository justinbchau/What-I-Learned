# Virtual environments

Why do we need them in Python? Simple. It's a good way to scope all the different Python libraries you install to a specific project instead of installing all these libraries globally. It only takes a couple different steps to set one up:

1.) First we create the virtual environment in your projects directory:

```python
$ pyton -m venv env

```

2.) Now that we've created one, we have to activate it with this command:

```python

$ source env/bin/activate

```

3.) You should now notice that the virtual environment is activated if you see that your command prompt is prefixed by the environment name you set like so:

```python

(env) $

```

It's now safe to install your Python libraries and it will only be scoped for this project! Enjoy :)
