# AlgorithmToRunESP32_SmartMethods
## Steps to run ESP32 Microcontroller


### First 

We have to install Arduino IDE on our computer 

### Second 

Open Arduino IDE and identifiy the port from > Tools > Port > COM4 

### Third 

Also from Tools > Go to Board Manager > Write ESP32 and choose the library 

* if you did not find the library 

Go to File > Preferences > Write in Additional Board Manager URLs : ```https://dl.espressif.com/dl/package_esp32_index.json``` 
to be able to download the library 

### Fourth

Go back to Tools > Go to Board Manager > Write ESP32 and choose the library and click on install

### Fifth 

Go to File > Examples > Basics > Choose blink and we will get this code 

``` 
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
} 
```

Click on Verify to check if there is error in the code 

Then 

Click on Upload to upload the code to the ESP32

### It will start to blink and run perfectly

