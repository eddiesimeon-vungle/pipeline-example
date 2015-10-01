# pipeline-example
[![Build Status](http://jenkins.vungle.com:8080/buildStatus/icon?job=pullrequest-pipeline-example)](http://jenkins.vungle.com:8080/view/system-integration/view/system-integration-jobs/job/pullrequest-pipeline-example/)

example pipeline

## build image locally

`ops/si-script.sh build`

## start service locally and then run tests

```
ops/si-script.sh startcontainers
ops/si-script.sh runtests
```

## jenkins job runs the following:
### builds image
`ops/si-script.sh build`
### tests image
`ops/si-script.sh test`
### tags and pushes image
`ops/si-script.sh tag`
