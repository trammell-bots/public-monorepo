# 000-moodbot

Minimal instructions for building the Rasa moodbot.


## To build and test

```console
python3 -m venv .venv
source .venv/bin/activate
pip3 install rasa==3.4 websockets==10.4
rasa --version
rasa data validate
rasa train
rasa test
```


## To clean up

```console
deactivate
rm -rf data/ models/ results/ tests/ .rasa/ .venv/ && rm -f *.yml
```


## Comments

It might be cleaner to move all this into a `Makefile`, using the tricks at e.g.
<https://stackoverflow.com/questions/33839018/activate-virtualenv-in-makefile>.



