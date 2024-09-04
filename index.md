# Learning Markdown on GitHub

![An image of Queer Pride](https://octodex.github.com/images/Octoqueer.png)

``` python
import time

input_hits = int(input("How many hits would you like to take?  "))
countdown = int(input("How long between hits? "))

def exe(hits):
    while hits > 0:
        input("Take a hit and press Enter")
        hits = hits - 1
        for x in range(countdown, 0, -1):
            seconds = x  % 60
            minutes = int(x / 60) % 60
            print(f"{minutes:02}:{seconds:02}")
            time.sleep(1)
        print("Time to hit it")
        print("Hits Remaining:", hits)

exe(input_hits)
print("You Win!")    

```
