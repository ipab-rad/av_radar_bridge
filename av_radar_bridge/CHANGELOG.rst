^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package av_radar_bridge
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.0.0 (2024-10-22)
------------------
* Update topics namespaces to match av_radar update
  - Input:  `/sensor/*` -> `/conti_pdk/*`
  - Output: `/output/*` -> `/sensor/*`
* Setting the correct network interface in Cyclone DDS configuration

* Contributors: Hector Cruz

1.1.0 (2024-05-21)
------------------
* Add cyclone DDS as ROS RMW  + configurate it to support high msg throughput
* Avoid `dev.sh` override `latest` docker tag for convenience
* Enable colorised ROS log
* Synchronise host time with docker container

1.0.0 (2024-05-01)
------------------
* Initial Radar configuration PR (`#1 <https://github.com/ipab-rad/av_radar_bridge/issues/1>`_)
  Setup Conti->Autoware radar msg pubsub bridge
  Pkg launches 16 composable nodes that subscribe to Continental's radar
  ecal_to_ros RadarDetectionImage msgs and publish the ROS standard
  radar_msgs RadarScan which Autoware consumes
* Upgrade Dockerfile w/ stages & convenient scripts
* Initial repo setup and WIP pubsub implementation
* Contributors: Alejandro Bordallo, Hector Cruz
