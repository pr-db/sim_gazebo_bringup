# sim_gazebo_bringup
# Installing ROS2
</br>You need to download this file inorder to install the ROS 
</br>https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXcfaeFblmznqth_0fk%2F-MXcgSRrBPzq5-K6O-C5%2Ffoxy_install_aim.sh?alt=media&token=2adf3a55-8463-4ff1-890e-67b6d32fe747
</br>RUN THE FOLLOWING COMMANDS
</br>cd ~/Downloads
</br>chmod a+x foxy_install_aim.sh
</br>./foxy_install_aim.sh
</br>source ~/.bashrc
# Installing Robocon Gazebo
</br>cd ~
</br>mkdir -p robocon_ws/src && cd robocon_ws/src
</br>git clone https://github.com/pr-db/sim_gazebo_bringup.git -b aim
</br>cd ~/robocon_ws
</br>colcon build --packages-select sim_gazebo_bringup --symlink-install
</br>echo "source /home/$USER/robocon_ws/install/setup.bash" >> ~/.bashrc
</br>source ~/.bashrc
</br>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py
