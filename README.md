# voting-app
Voting-app for Kubernetes deployment

# clone the project on local system.
$ git clone https://github.com/anishraut7836/voting-app.git 
# create docker image for worker app and push it to docker registory
$ cd voting-app
$ cd worker
$ docker build -t anishraut7836/worker-app:1 .
$ docker push anishraut7836/worker-app:1

# create docker image for vote app and push it to docker registory
$ cd ../vote
$ ls -l
$ docker build -t anishraut7836/vote-app:1 .
$ docker push anishraut7836/vote-app:1

# create docker image for result app and push it to docker registory
$ cd ../result
$ ls -l
$ docker build -t anishraut7836/result-app:1 .
$ docker push anishraut7836/result-app:1
