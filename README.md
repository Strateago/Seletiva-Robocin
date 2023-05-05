# Seletiva-Robôcin
Ros2 workspace usado para desafio da seletiva-2023 do RobôCin

Foi necessario compactar por causa do número de arquivos no workspace, logo para usar é necessário descompactar


# Instalar opencv:

pip install imutils

pip install numpy

pip install opencv-python


# Configurando o workspace e setando o caminho na .bash:

No diretório "ros_ws", digite no terminal: colcon build

Adicione no final do arquivo .bash: "source /CAMINHO DA PASTA "ROS_WS"/install/setup.bash"

No terminal digite: "source ~/.bashrc"

Agora você pode utilizar o comando para executar o código de qualquer tmerminal

# Para executar:

Abra o mapa "quadrado_seletiva.world" no gazebo

Abra o QGround

Execute em terminais diferentes: 

sim_vehicle.py -v ArduCopter -f gazebo-iris --no-mavproxy

mavproxy.py --master tcp:127.0.0.1:5760 --out 127.0.0.1:14550 --out 127.0.0.1:14551

ros2 run drone_camera recieve_image
