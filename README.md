# git

## Links
* [Push a new local branch to a remote Git repository and track it too](https://www.freecodecamp.org/forum/t/push-a-new-local-branch-to-a-remote-git-repository-and-track-it-too/13222/1)

## Commands
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

## Git URLs
The native transport (i.e. git:// URL) does no authentication and should be used with caution on unsecured networks.

The following syntaxes may be used with them:
       o   ssh://[user@]host.xz[:port]/path/to/repo.git/
       o   git://host.xz[:port]/path/to/repo.git/
       o   http[s]://host.xz[:port]/path/to/repo.git/
       o   ftp[s]://host.xz[:port]/path/to/repo.git/

An alternative scp-like syntax may also be used with the ssh protocol:
       o   [user@]host.xz:path/to/repo.git/

       This syntax is only recognized if there are no slashes before the first colon. This helps differentiate a
       local path that contains a colon. For example the local path foo:bar could be specified as an absolute path or
       ./foo:bar to avoid being misinterpreted as an ssh url.

       The ssh and git protocols additionally support ~username expansion:

       o   ssh://[user@]host.xz[:port]/~[user]/path/to/repo.git/

       o   git://host.xz[:port]/~[user]/path/to/repo.git/

       o   [user@]host.xz:/~[user]/path/to/repo.git/

       For local repositories, also supported by Git natively, the following syntaxes may be used:

       o   /path/to/repo.git/

       o   file:///path/to/repo.git/

       These two syntaxes are mostly equivalent, except when cloning, when the former implies --local option. See
       git-clone(1) for details.

       When Git doesn't know how to handle a certain transport protocol, it attempts to use the remote-<transport>
       remote helper, if one exists. To explicitly request a remote helper, the following syntax may be used:

       o   <transport>::<address>

       where <address> may be a path, a server and path, or an arbitrary URL-like string recognized by the specific
:
