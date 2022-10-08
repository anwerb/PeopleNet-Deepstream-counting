make sure to clone this repository in /opt/nvidia/deepstream/deepstream/sources with direct access to project folder (remove PeopleNet-Deepstream-counting folder).

make a new folder in project directory :
/opt/nvidia/deepstream/deepstream/sources/project$ sudo mkdir data

you can download any mp4 / h264 file in there and use it for inference ( don't forget to change the default 'cctv.mp4' file name in configs/project_base_config_peoplenet.txt )

update the crossing lines in configs/analytics_config.txt for the desired usecase ( you can use KRuler to determine which pixels are which in each video you use )

to do: fixing kafka broker communication in configs/project_base_config_peoplenet.txt .

for live inference ( with bounding boxs )
change [sink0] property "type" to 2.

for output file ( with bounding boxs )
change [sink0] property "type" to 3 and name the output file to your liking.
