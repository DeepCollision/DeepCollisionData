# DeepCollision REST API Example

> This document is an example demonstrating how to use **DeepCollision REST APIs** for environment parameter configurations.<br/> 
> You can refer it to write your own Python programs.

### Step 1: Load scene and generate AVUT's position

There are a two parameters in **LoadScene API**: the first one is Map, and the second one is the road which the AVUT will drive on.

```python
import request
requests.post("http://119.45.188.204:5000/LGSVL/LoadScene?scene=SanFrancisco&road_num=1")
```

### Step 2: Configure the operating environment

Set rain level to light rain.

```python
requests.post("http://119.45.188.204:5000/LGSVL/Control/Weather/Rain?rain_level=Light")
```

### Step 3: Get state returned

```python
    r = requests.get("http://192.168.50.81:5000/LGSVL/Status/Environment/State")
    a = r.json()
    #### State returned after one configuration action executed.
    state = np.zeros(12)
    state[0] = a['x']
    state[1] = a['y']
    state[2] = a['z']
    state[3] = a['rain']
    state[4] = a['fog']
    state[5] = a['wetness']
    state[6] = a['timeofday']
    state[7] = a['signal']
    state[8] = a['rx']
    state[9] = a['ry']
    state[10] = a['rz']
    state[11] = a['speed']
```

