This repo is to test the OOM exception being thrown while using multiple package directories. Below are the steps to reproduce the error  :

1. Create an org usig sfdx force:project:create command.
2. Execute force:source:status and force:source:push and push the files into the org.
3. Modify a file withing each package directory.
4. Execute force:source:status again. You will get the Out of Memory execption error.