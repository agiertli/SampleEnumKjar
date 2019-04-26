Repository Init Content
=======================

Your project description here.

jenkins need more resources:

oc new-app jenkins-persistent --param ENABLE_OAUTH=true --param MEMORY_LIMIT=2Gi --param VOLUME_CAPACITY=4Gi


even then, it will incredibly slow from the beggining, but should get better with time