# Jenkinsfile_NodeJS_Example

1. Install Git on CentOS/any machine: Follow this: https://linuxize.com/post/how-to-install-git-on-centos-7/

2. In Jenkins, Install Git plugin then go to manage Jenkins -> Global tool configuration-> Git-> Name: Default, Check ‘Install automatically’ if you don’t have installed in your machine or virtual instance, Path to Git Executable: Git  

3. In Jenkins, go to manage Jenkins -> Global tool configuration-> NodeJS-> Name: node, Check ‘Install automatically’, select the version from dropdown and left the other fields as it is. Jenkins will take care NodeJS installation.  

4. Create new Job: New Item -> Pipeline Script

5. GitHub project: Project URL: https://github.com/hossain434/nightwatch_sample_example

6. Pipeline: Definition-> Pipeline script form SCM

    SCM-> Git

    Repository URL: https://github.com/hossain434/nightwatch_sample_example  (doesn’t need to provide .git URL)

    Left the credentials blank since this is public link

    Branch to build: Master

    Repository browser: Auto

    Script path: Jenkinsfile

    Create a Jenkinsfile and add in the GitHub project. If you have more than one then name as Jenkinsfile_1, Jenkinsfile_2 etc.

    Example: https://github.com/hossain434/InvoicePdfkitNodeJs/blob/master/Jenkinsfile

    Build Trigger: Setup schedule.

    #### Reference: https://medium.com/@gustavo.guss/jenkins-starting-with-pipeline-doing-a-node-js-test-72c6057b67d4
