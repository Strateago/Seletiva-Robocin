# Seletiva-Robocin
Ros2 Node usado para desafio da seletiva-2023 do RoboCin


# Necessário opencv instalado:

pip install imutils

pip install numpy

pip install opencv-python


# Também é necessário atualizar a .bashrc com o setup do workspace do ros2, adicionando:

source ~/ros2_ws/install/setup.bash


# Para executar:

Abra o mapa "quadrado_seletiva.world" no gazebo

Abra o QGround

Execute em terminais diferentes: 

sim_vehicle.py -v ArduCopter -f gazebo-iris --no-mavproxy

mavproxy.py --master tcp:127.0.0.1:5760 --out 127.0.0.1:14550 --out 127.0.0.1:14551

ros2 run drone_camera recieve_image
