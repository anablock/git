# git
* ls -l
* git add --all
* chmod 644 onb_ApplicationFormController.js
* git checkout develop onb_ApplicationFormController.js
* git checkout onb
* git fetch origin
* sfdx force:org:list
* sfdx force:source:deploy -p src/classes/onb_RegisterEntityDetailsControllerTest.cls -u OnbSandbox
* cp /tmp/tmp/sfdx-project.json .
* popd
* sfdx force:project:create -n tmp
* pushd /tmp
* vi sfdx-project.json
* cat > sfdx-project.json
* code src/classes/onb_RegisterEntityDetailsControllerTest.cls
* cd ~/Projects/salesforce/
* git checkout -b my_branch
* cat deploy.sh  - to deploy 
* sfdx force:mdapi:deploy -d src/ -u staging --testLevel=RunLocalTests (add wait flag to get errors)

* sfdx force:apex:test:run [-n <array> | -s <array> | -t <array>] [-c] [-d <directory>] [-l 
  RunLocalTests|RunAllTestsInOrg|RunSpecifiedTests] [-w <minutes>] [-y] [-r human|tap|junit|json] [-u <string>] 
  [--apiversion <string>] [--verbose] [--json] [--loglevel trace|debug|info|warn|error|fatal]


* sfdx force:apex:test:run -u vuk.djukic_external.k2@coinbase.com.staging --testlevel=RunLocalTests

* sfdx force:auth:jwt:grant --clientid $HUB_CONSUMER_KEY --jwtkeyfile file.key --username  -r $SALESFORCE_DOMAIN
