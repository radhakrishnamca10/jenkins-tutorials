# jenkins-tutorials
This is for Jenkins part of DevOps Classes

Before executing Jobs, Manual configuration to be done on the Linux server where jenkins is installed.

By default Jenkins installation creates a user called `jenkins` and all jenkins jobs would be executed with that user, so I have enabled the sudo access to the `jenkins` user by updating `visudo`

        i)    Login to RHEL-8 EC2
        ii)   sudo visudo -> update the sudoers with entry `jenkins	ALL=(ALL) 	NOPASSWD: ALL`
        iii)  Now Jenkins Pipelines should be able to function normally without issues


#Jenkins_Syllabus

`1. Installation of Jenkins`

      i)      Theory of Jenkins
      ii)     Dependent on Java
      iii)    Install Jenkins on RedHat8 Linux (AWS EC2 Instance)
      iv)     Access Jenkins via browser
      v)      Tour of Jenkins
      vi)     Create View/Folder

`2. Administration of Jenkins`

      i)      Plugins and installation of plugins
      ii)     Manage Jenkins
      iii)    Users creation and permissions
      iv)     Jenkins config file  ```/var/lib/jenkins```
      v)      Jenkins Slaves and Adding nodes to Jenkins master
      vi)     Labels and use labels in the pipelines (covered during pipeline topic)

`3. Jobs Creation`

      i)      Structure of Jenkins Jobs
      ii)     Freestyle Job creation
      ii)     Adding Parameters to Jobs
      iii)    Build Environment variables
      iii)    Different types of Jobs
      iv)     Greenballs plugin
      vi)     Debugging/troubleshooting Jobs
      vii)    Exploring Jobs on Linux Box
      viii)   Adding Source control to Jobs

`4. Git push/PR to trigger Jobs`

      i)      Integrating Git with Jenkins
      iii)    Trigger jobs with Git Push/Pull Request    

`5. Pipeline Jobs and Jenkinsfile`

      i)      Installing Pipeline Plugin
      ii)     Types of Pipelines Scripted & Declarative
      iii)    Structure of Pipeline Job
      iv)     Create Pipeline Jobs
      iv)     Adding Jenkinsfile to Pipeline Job
      v)      Pipeline to execute ANSIBLE PLAYBOOK
      vi)     Pipeline to execute Terraform code

`6. Moving Jobs from one jenkins to another jenkins`

`7. Groovy examples with realtime process of mother seed job and configuration Jobs` (NOT MANDATORY)
