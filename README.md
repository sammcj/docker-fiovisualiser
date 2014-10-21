## docker-fiovisualiser

Run fiovisualiser in a headless docker container accessible via an HTML5 noVNC connection

The noVNC container is based off dit4c/dockerfile-dit4c-container-x11

### Usage

1. Build the image
```
docker build . -t docker-fiovisualiser
```
2. Run the container
```
docker run -i -t -p 8080:8080 docker-fiovisualiser
```
3. Browse to http://serverip:8080
4. Run the noVNC session
5. Run `cd fiovisualiser && python fiovisualiser.py`

### Screenshot

![screen shot 2015-08-13 at 15 08 39](https://cloud.githubusercontent.com/assets/862951/9242978/403ba2dc-41cd-11e5-949f-f40bf7c8ec30.jpg)

Credits:

- https://github.com/dit4c
- https://github.com/01org/fiovisualizer
