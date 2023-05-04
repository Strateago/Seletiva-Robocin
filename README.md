# Seletiva-Robôcin
Ros2 workspace usado para desafio da seletiva-2023 do RobôCin

Foi necessario compactar por causa do número de arquivos no workspace, logo para usar é necessário descompactar


# Instalar opencv:

pip install imutils

pip install numpy

pip install opencv-python


# Atualizar a .bashrc com o setup do workspace do ros2, adicionando:

source ~/ros2_ws/install/setup.bash


# Para executar:

Abra o mapa "quadrado_seletiva.world" no gazebo

Abra o QGround

Execute em terminais diferentes: 

sim_vehicle.py -v ArduCopter -f gazebo-iris --no-mavproxy

mavproxy.py --master tcp:127.0.0.1:5760 --out 127.0.0.1:14550 --out 127.0.0.1:14551

ros2 run drone_camera recieve_image
