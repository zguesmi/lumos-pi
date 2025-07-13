# LumosPi - An assistant for blind persons
![logo](./logo.png)

### TODO:
https://github.com/facebookresearch/Detectron

## Description
An assistive system for visually impaired individuals using a Raspberry Pi, ultrasonic sensors, and a camera to enable obstacle detection and text recognition.

### Main Features
**Avoid obstacles:** ultrasonic sensors are used to detect obstacles and warn the user through earphones.

**Read documents:** we take pictures of documents and we use OCR to extract text from those images and convert it to speech.

## Dependencies
- [python3](https://www.python.org/)  
- [tesseract-ocr](https://github.com/tesseract-ocr/tesseract)  
- [opencv](https://opencv.org/)

## Usage
To use the project first insure that you have all dependencies installed then run the main python script.

    # install dependencies
    $ sudo apt update && sudo apt install -y tesseract-ocr tesseract-ocr-eng python3 python3-pip

    $ git clone https://github.com/Zied-Guesmi/blind-assistant.git && cd blind-assistant/
    $ pip3 install -r requirements.txt
    $ python3 src/main.py


## Docker deployment
After installing [docker](https://docs.docker.com/install/), just grab the docker image from dockerhub and run it:

    $ docker run ziedguesmi/blind-assistant

Or you can build your own image from dockerfile:

    # clone the project
    $ git clone https://github.com/Zied-Guesmi/blind-assistant.git && cd blind-assistant/

    # build the docker image
    $ docker build -t blind-assistant .

    # run the container
    $ docker run blind-assistant

## License
This project is licensed under the GPLv2 License - see the [LICENSE](https://github.com/Zied-Guesmi/blind-assistant/blob/master/LICENSE) file for details.


## TODO
- Support more languages.
