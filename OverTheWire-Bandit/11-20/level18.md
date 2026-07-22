
Goal: To retrieve password stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

Commands used:
  - ```ssh -t``` with ```bash --norc```

Procedure:
  - Since the ```.bashrc``` is customised to immediately log us out, we will have to find a way to disable this customisation whilst retaining a terminal we can interact with.
  - To achieve this, ```-t``` flag is useful for creating an instance of an interactable terminal, while the ```bash --norc``` flag is useful for not executing the customisation in the ```.basrc```.
  - With access to the server now, ```cat readme``` does the trick of giving us the answer.

Learnings:
  - Yet another flag and usage of ssh connection.
  - This method can probably be used for debugging too, besides forcing an entry into connecting.

