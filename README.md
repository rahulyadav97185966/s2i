# s2i

1) oc new-project mypro  : create a project of any name mypro
2) create a new application using following command
3) oc new-app --name=myweb https://github.com/rahulyadav97185966/index  :: paste the github link here or any link to create a project
4) Now the applications is created and we can run that using following commands
5) when we create a application it automatically get the page related to it.
6)  2  oc new-project mypro
    3  oc new-app --name=website https://github.com/rahulyadav97185966/index
    4  oc get pods
    5  oc get pods -o wide
    6  oc expose service website
    7  oc get route
    8  oc get svc
    9  curl 172.30.70.4:8080  : you will get the website
    #if code is changed
   10  git clone https://github.com/rahulyadav97185966/index :: create a clone or copy the files from website
   11  ls
   12  cd index/
   13  ls
   14  vi index.php
   15  git commit -m "hello" index.php
   16  git add .
   17  git push origin master
   18  oc start-build website :  it rebuild the site and and versions are maintained in docker-registry and the path is saved in openshift
   19  oc get pods
   20  oc get pods -w
   21  oc get svc
   22  curl 172.30.70.4:8080
   
