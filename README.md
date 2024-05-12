# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
Developed by: MERCY A
RegisterNumber: 212223110027
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)

```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/mercyarulappan/Movement-of-Robot-Joints/assets/149233730/19865e92-3b12-4dfd-a93a-bd24571e0b37)

### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/mercyarulappan/Movement-of-Robot-Joints/assets/149233730/0a2b9cd9-f88d-4de7-a9fe-82a2b06408ac)

### 3. Movement of Joint1

![image](https://github.com/mercyarulappan/Movement-of-Robot-Joints/assets/149233730/19c8e29b-2528-4e9f-8778-da739c42b87a)

### 3. Movement of Joint2

![image](https://github.com/mercyarulappan/Movement-of-Robot-Joints/assets/149233730/2760a4d0-3b3c-45b3-a28c-b6c32fc9163c)

### 3. Movement of Joint3

![image](https://github.com/mercyarulappan/Movement-of-Robot-Joints/assets/149233730/062498a6-db7a-48da-8f17-1e379fc0960a)

## Result 
Thus the different robots joints are moved with the help of python list.


