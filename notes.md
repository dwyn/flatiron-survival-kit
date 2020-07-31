MY_PAT=eyp63idpxren5qy2rwygm7hh4ut4dvj52zxnfuuwwiammkvuez7q
B64_PAT=$(echo ":$MY_PAT" | base64)
git -c http.extraHeader="Authorization: Basic ${B64_PAT}" clone git@github.com:dwyn/flatiron-survival-kit.git

curl -u username[:{eyp63idpxren5qy2rwygm7hh4ut4dvj52zxnfuuwwiammkvuez7q}] https://dev.azure.com/dwyn/_apis/build-release/builds