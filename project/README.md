make sure to clone this repository in /opt/nvidia/deepstream/deepstream/sources with direct access to project Folder (remove PeopleNet-Deepstream-counting)

make a new Folder in project directory :
/opt/nvidia/deepstream/deepstream/sources/project$ sudo mkdir data

you can download any mp4 / h264 file in there and use it for inference ( don't forget to change the default 'cctv.mp4' file name in configs/project_base_config_peoplenet.txt )

update the crossing lines in configs/analytics_config.txt for the desired usecase ( you can use KRuler to determine which pixels are which in each video you use )
