Guacamole-demo
====

I heard that running ssh in a container is a bad thing.  OK,
here is my solution.  A full X session. HA

Just a simple example of using my hall\guacamole image.

---
Author
===

Randy Hall <randy.hall@open-source.guru>

---
Building
===

Build from docker file:

```
git clone git@github.com:hall757/guacamole.git
cd guacamole/demo
docker build -t guacamole-demo . 
```

---
Running
===

On a secure network, launch with the following.

```
docker run -d -p 8080:8080 guacamole-demo
```

Browse to ```http://your-host-ip:8080```
Username: demo
Password: demo
