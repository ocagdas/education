# education
basic ubuntu build, test, education playground

# docker build
```
docker build -f ./DockerfileEducation -t zmart/education .
```

# to run
```
docker run --rm -it --net=host --name edu_`whoami`_`date +%s` -e uid=`id -u` -v`pwd`:/export zmart/education /bin/bash
docker run --rm -dit --name edu_`whoami`_`date +%s` -e uid=`id -u` -v`pwd`:/export zmart/education /bin/bash -c '/etc/init.d/ssh start && /bin/bash'
```

# to change the ssh passwd later
```
ssh ssher@172.17.0.2 'echo "ssher:newpass123" | sudo chpasswd'
```

