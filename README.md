# ros2_stack_sim_jackal

## Para instalar y correr este proyecto
1. Clona el repositorio dento de tu directorio ```ros2_ws/src/```
2. Instalar el stack de navegación de ROS2 ```sudo apt install ros-humble-navigation2 ros-humble-nav2-bringup```
3. Instala los paquetes del Jackal: ```sudo apt install ros-humble-clearpath-desktop sudo apt-get install ros-humble-clearpath-simulator sudo apt-get install ros-foxy-jackal-simulator ros-foxy-jackal-desktop ros-foxy-jackal-navigation```
4. Revisa si te falta instalar alguna dependencia: ```rosdep install -i --from-path src --rosdistro humble -y``` (debes estar dentro de tu directorio ```ros2_ws/``` para poder correr el comando).
5. Compilar usando ```colcon_build``` estando ubicando dentro de ```ros2_ws/``` (debería de compilar correctamente el paquete de ROS)
6. Ir al paquete usando ```roscd ros2_stack_sim_jackal``` y después ir a ```cd src/```
7. Modificar los permisos del archivo ```env_run``` para que tenga permisos de ejecución ```sudo chmod +x env_run```
8. Correr el launch file ```simulation2d.launch```