# Projet 3 INF3995 - Équipe 103

# Prerequisites
* [Docker](https://docs.docker.com/get-docker/)
* [Docker Compose](https://docs.docker.com/compose/install/)
* [x11Docker](https://github.com/mviereck/x11docker)

# Cloner the repo

```
git clone --recurse-submodules https://gitlab.com/polytechnique-montr-al/inf3995/20221/equipe-103/INF3995-103.git
```

## Video demos

1. [RF2 RF3 RF4 RF5 RF6 RF7 RF8 RF9 et RF11 (physique)](https://youtu.be/435cvL4hRAc) MAIN ONE!!

2. [RF2 et RF4 (simulation)](https://youtu.be/DDPy3zP6av8)

3. [RF2 (physique)](https://youtu.be/0ldOjo93YiA)

4. [RF3 (simulation)](https://youtu.be/6V3i5QbMqSM)

5. [RF3 (physique)](https://youtu.be/6oj3N6FtFUk)

6. [RF4 (physique)](https://youtu.be/0ldOjo93YiA)

7. [RF5 (simulation)](https://youtu.be/_wsYKvkqE_U)

8. [RF5 (physique)](https://youtu.be/0ldOjo93YiA)

9. [RF6 (simulation)](https://youtu.be/ZjJxnp08VyY)

10. RF7 (simulation):https://youtu.be/HtsJeYMvS48 et https://youtu.be/f4pQGaMIH9o

11. [RF8 RF9 et RF11 (simulation):](https://youtu.be/wgHPegepmkc)

12. [RF10 (RR)](https://youtu.be/gvLCnpMKphQ)

13. [RF13](https://youtube.com/shorts/S4xfAArf5-k?feature=share)

14. [RF17 et RF18 (simulation)](https://youtu.be/cMP4kRYs6wc)

15. [RF17 et RF18 (physique)](https://youtu.be/hpVkW4-mHgo)

16. [RC1 (simulation)](https://www.youtube.com/watch?v=EOlxl1FAvlE)

17. [RC1 (physique)](https://youtu.be/ZCaThBH-fKE)

19. [RC2:](https://youtu.be/ZYtIfvIZdOM)

19. [RC3:](https://youtu.be/fqE2uKaNJmc)

20. [RC5:](https://youtu.be/0Ivn4ZESiYs)

# To start the project
```
./start.sh
```

## Frontend

Built with Angular.

To run it using docker compose:
```
docker-compose up --build Interface
```
Or without docker compose:

```
cd Interface
npm install
ng add @angular/material
npm install firebase @angular/fire --save
npm install duration
ng serve –open
```

## Backend


Built with Flask(Python)

Run it with docker compose:
```
docker-compose up --build server
```
Or without docker compose:

```
cd Server
pip3 install pipenv
virtualenv nomEnv
source nomEnv/bin/activate
pip3 install flask
pip3 install flask-cors
pip3 install -r requirements.txt
```

Then run it :
```
python3 src/main.py
```

## Crazyflie-firmware
This is the firmware for our crazyflie drone

## Simulation
### Note: Before running the following commands, make sure the frontend and backend are already running

Run it with docker compose:
```
docker-compose up --build simulation
```
Then run the script sim_launch.sh in the simulation folder
```
./simulation/sim_launch.sh
```

Press the play button

# Coding style

- ## Typescript: [Google Typescript Style Guide](https://google.github.io/styleguide/tsguide.html)

- ## C: [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)

- ## Python: [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)
