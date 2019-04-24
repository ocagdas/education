# education
basic ubuntu build, test, education playground

# docker build
```
docker build -f ./DockerfileEducation18.04 -t zmart/education-18.04 .
```

# to run
```
docker run -dit --name edu zmart/education:latest
```

# to change the ssh passwd later
```
ssh ssher@172.17.0.2 'echo "ssher:newpass123" | sudo chpasswd'
```

