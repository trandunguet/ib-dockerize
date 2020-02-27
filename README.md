Edit the id and password in IBController.ini and then:

```
$ sudo docker image build -t ib-controller-run .
$ sudo docker container run -it --rm -e DISPLAY=${DISPLAY} -v /tmp/.X11-unix:/tmp/.X11-unix ib-controller-run
$ /opt/IBController/IBControllerGatewayStart.sh
```
