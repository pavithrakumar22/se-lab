//maven java

new item

maven_build  
freestyle project
git

branches to buid */main

in build triggers
select pollscm
*****


build steps

add build steps
invoke top level maven targets
maven home
clean

add build steps
invoke top level maven targets
maven home
install

add post build action
archive artifacts
**/*

build other projects
maven_test

same
none
delete workspace before build starts

add build steps
copy artifacts from other project
stable build only
**/*
add build steps
invoke top level maven targets
maven home
test

add post build actions
build other projects
deploy

build steps
maven_test
**/*

post build
deploy war/ar to container
**/* .war
add credentials



create pipeline
maven-pipleine
build pipeline view
