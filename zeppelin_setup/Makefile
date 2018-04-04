.PHONY: help

build_zeppelin: # run it to build the image 
	docker build -t ubuntu:zeppelin .

start_zeppelin_current_dir_mount: # run this to start the zèppelin notebook with persistent volume ${PWD}
	docker run  --rm -it -p 8080:8080 -v ${PWD}:/zeppelin/notebook/  ubuntu:zeppelin 
# in order to recover your data every time use the same vdirectory

