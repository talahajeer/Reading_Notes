# Big O notation
 Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.

 A grasp of Big O is an important tool when dealing with algorithms that need to operate at scale, allowing you to make the correct choices and acknowledge trade-offs when working with different data sets.

![Big O notation](https://miro.medium.com/max/1400/1*FkQzWqqIMlAHZ_xNrEPKeA.png)


# Python Environment for Data Science
 Pyenv is a set of three tools, from which I present two here, that are pyenv (used to install python) and pyenv-virtualenv (used to configure your global tools). You can install them by
 ``curl https://pyenv.run | bash``
 After that, add the following lines to your .bashrc (same for .zshrc) to have pyenv available in your terminal
 ``export PATH="~/.pyenv/bin:$PATH"``
 ``eval "$(pyenv init -)"``
 ``eval "$(pyenv virtualenv-init -)"``

 And finally, restart your terminal. Now, you can use pyenv to install almost any python interpreter, including pypy, and anaconda. Note, that pyenv builds python locally on your machine. Building python requires several libraries.