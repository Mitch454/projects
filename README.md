# Startpage

This is a simple start page, to scrub up on css.

## Heading 2

I suppose it might also be time to learn how to write **markdown**.


### This is a quoteblock

> We trust you have received the usual lecture from the local System Administrator.
> It usually boils down to these three things:
>    1. Respect the privacy of others.
>    2. Think before you type.
>    3. With great power comes great responsibility.




## Heading 2

  * unordered lists
  * are almost as cool
  * as ordered lists



### Here is a codeblock

~~~python
import random
from time import sleep as s

def randomSleep(num):
    randWaits = random.uniform(num, (num + 1))
    randWaits = float(("{:.6f}".format(round(randWaits, 6))))
    print("waiting " + str(randWaits) + "s..")
    s(randWaits)
~~~


