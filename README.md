## Hello, Apps! ##

A sample app that is built using the S2I golang builder..


```bash
curl 10.1.0.2:8888
```
To test from external network, you need to create router. Please refer to [Running the router](https://github.com/openshift/origin/blob/master/docs/routing.md)

The container doesn't expose any ports, this will require you to expose it manually.
For example:

```bash
oc expose dc/goapps --port=8888
```
   

and lastly if you want to expose a route, by doing:
```bash
oc expose service/goapps
```
