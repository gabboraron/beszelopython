# Hang alapú értesítés ha programunk lefutott
> bővebben: https://stackoverflow.com/questions/16573051/sound-alarm-when-code-finishes

# Szükséges hozzá:
Szükséges a `sox` ami beszerezhető: `sudo apt install sox`

# Hangjelzés
````Python
import os
duration = 1  # seconds
freq = 440  # Hz
os.system('play -nq -t alsa synth {} sine {}'.format(duration, freq))
````

# Szöveggel
````Python
import os
os.system('spd-say "your program has finished"')
````
