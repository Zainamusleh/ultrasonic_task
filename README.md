# ultrasonic_task

A task to make an alarm system using ultrasonic
<img src="https://th.bing.com/th/id/R.8d3b64744912305e876c2fcfb6213e65?rik=cVNE1tGmhtNfRg&pid=ImgRaw&r=0" alt="Employee data" title="Employee Data title" width="200" >

<img src="https://th.bing.com/th/id/R.2ae1fd15ec012a7b1763edf99c38dd5a?rik=eHYPn7i9krthSA&pid=ImgRaw&r=0" alt="Employee data" title="Employee Data title" width="200" >


**** Code explaining:****
```
# Define two objects: a DistanceSensor and a Buzzer
ultrasonic = DistanceSensor(echo=17, trigger=4)
buzzer = Buzzer(2)

# Main program loop that runs continuously
while True:
    # Read the distance and print it to the console
    distance = ultrasonic.distance * 100  # Convert distance from cm to m
    print(distance)
    
    # Turn on the buzzer if the calculated distance is less than or equal to 10 cm
    if distance <= 10:  # Check if distance is less than or equal to 10 cm
        buzzer.on()  # Turn on the buzzer
    # Turn off the buzzer if the calculated distance is greater than 10 cm
    else:
        buzzer.off()  # Turn off the buzzer

```


Team:
* [Hala](@hala214)
* [Tala](@talashweiki)
