A computer vision bot for the mini fishing game in metin2.<br>
It uses mainly OpenCV and an Arduino to send mouse commands.

![Preview](/preview.gif)

# How to run

Install Package
```shell
pip install .
```

## Arduino Leonardo
If you want to use the Arduino Leonardo, connect it trough a USB port and upload ```Arduino/leonardo_mouse_relay.ino```.
Whenever executing metinfishingbot the flag ```--use_arduino``` needs to be passed.


## Diferent run methods
Display the vision of the bot from the example video in a new window
```shell
metinfishingcv --video video_samples\\fishing_data_test.mp4 --debug
```

Display the vision of the bot only for the fish
```shell
metinfishingcv --video video_samples\\fishing_data_test.mp4
```

Run the bot on the window "Metin" and display it's vision
```shell
metinfishingbot Metin
```

Run the bot, using an arduino for mouse simulation, on the window "Metin" and display it's vision
```shell
metinfishingbot Metin --use_arduino
```

Run the bot on the window "Metin" synchronously without displaying the image and resize the frame to 0.7 
```shell
metinfishingbot Metin --fast --resize_factor 0.7
```
