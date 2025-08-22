# Bluetooth-Smart_Car
This is a bluetooth smart car which can detect and avoid obstacles and steer clear off its path using four IR sensors and one Ultrasonic sensor on top of a micro servo.
It is controlled by HC-05 Bluetooth Module and uses L298N Motor Driver Circuit along with an arduino UNO R3.
It's a simple project made by me on my free time.
# Modules & Hardware Used
Arduino Board (any compatible)
L298N Motor Driver Module
Servo Motor (for sensor rotation)
Ultrasonic Distance Sensor (HC-SR04 or similar)
Four IR Sensors (for left, right, left-back, and right-back)
Two DC Motors (for robot wheels)
# How It Works
Reads sensor inputs to decide movement or avoidance actions.
Accepts direct commands over Serial for user control.
Avoids obstacles by stopping, scanning side distances, and choosing the safer direction.
IR sensors detect drop-offs or line edges, causing the car to halt or turn automatically.

# Customization
Adjust sensor pins and logic to match your own robot configuration.
Expand functionality by adding more sensors or integrating camera/image processing.
Tweak movement logic for different drive setups.

PS: please don't plug the bluetooth module while uploading as it creates issues with the TTL logic of code upload.
# Sensor/Component	    Arduino Pin	Description
Left Motor Forward	    5	L298N motor driver control pin
Left Motor Backward	    4	L298N motor driver control pin
Right Motor Forward	    3	L298N motor driver control pin
Right Motor Backward	  2	L298N motor driver control pin
Left IR Sensor        	9	Digital input for left IR sensor
Right IR Sensor	       10	Digital input for right IR sensor
Left Back IR Sensor   	6	Digital input for left back IR
Right Back IR Sensor   	7	Digital input for right back IR
Ultrasonic Sensor Trig	A3	Analog pin (Trig) for distance sensor
Ultrasonic Sensor Echo	A2	Analog pin (Echo) for distance sensor
Servo Motor Control	    11	PWM pin for servo motor control

