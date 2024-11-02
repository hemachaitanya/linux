

#### File and Folder Management

```text

1. Create file: touch filename
2. Create folder: mkdir foldername
3. Create multiple folders: mkdir -p folder1/folder2/folder3
4. Delete file: rm filename
5. Delete folder: rmdir foldername (only works if folder is empty)
6. Delete folder and contents: rm -rf foldername
7. Copy file: cp source destination
8. Move/Rename file: mv source destination
9. List files/folders: ls [options] (e.g., ls -l, ls -a)
```

#### Permissions

```text

1. Change ownership: chown user:group filename
2. Change permissions: chmod permissions filename (e.g., chmod 755 filename)
3. Add permissions: chmod +x filename (execute permission)
4. Remove permissions: chmod -x filename (execute permission)
```
#### User and Group Management

```text
1. Create user: useradd username
2. Create user with group: useradd -g groupname username
3. Delete user: userdel username
4. Create group: groupadd groupname
5. Delete group: groupdel groupname
6. Add user to group: usermod -aG groupname username
7. Remove user from group: gpasswd -d username groupname
8. Change user's primary group: usermod -g groupname username
9. List users: getent passwd or cat /etc/passwd
10. List groups: getent group or cat /etc/group
```

#### Automation Examples

```text

1. Create 5 users with same group:


for i in {1..5}; do useradd -g mygroup user$i; done

1. Create 10 folders with specific permissions:


for i in {1..10}; do mkdir folder$i; chmod 755 folder$i; done

1. Delete all files in a folder:


find /path/to/folder -type f -delete

1. Change ownership of all files in a folder:


chown -R user:group /path/to/folder

Scripts and Automation Tools

```
#### [12:06 am, 3/11/2024] Meta AI: Jenkins CLI Commands

1. List all jobs: jenkins-cli list-jobs
2. Build a job: jenkins-cli build job_name
3. Get job status: jenkins-cli get-job job_name
4. Update job configuration: jenkins-cli update-job job_name
5. Delete a job: jenkins-cli delete-job job_name
6. List all nodes: jenkins-cli list-nodes
7. Connect to node: jenkins-cli connect-node node_name
8. Disconnect node: jenkins-cli disconnect-node node_name

Jenkins Pipeline Commands

1. Trigger pipeline: jenkins-cli build pipeline_name
2. Get pipeline status: jenkins-cli get-pipeline pipeline_name
3. Update pipeline configuration: jenkins-cli update-pipeline pipeline_name

Problem-Solving Commands

Build Issues

1. Check build logs: jenkins-cli build logs job_name
2. Check console output: jenkins-cli console-output job_name
3. Run Groovy script: jenkins-cli groovy script.groovy

Node Issues

1. Check node status: jenkins-cli node-status node_name
2. Restart node: jenkins-cli restart-node node_name
3. Update node configuration: jenkins-cli update-node node_name

Plugin Issues

1. List installed plugins: jenkins-cli list-plugins
2. Install plugin: jenkins-cli install-plugin plugin_name
3. Update plugin: jenkins-cli update-plugin plugin_name

Authentication Issues

1. Authenticate user: jenkins-cli authenticate username password
2. Create API token: jenkins-cli create-api-token username
3. Update API token: jenkins-cli update-api-token username

Common Jenkinsfile Steps

1. Define pipeline: pipeline { ... }
2. Define stage: stage('Stage Name') { ... }
3. Define step: step('Step Name') { ... }
4. Use environment variables: env.VARIABLE_NAME
5. Use credentials: withCredentials([usernamePassword(...)]) { ... }

Troubleshooting Jenkins

1. Check Jenkins logs: /var/log/jenkins/jenkins.log (Ubuntu-based)
2. Check system logs: dmesg | grep jenkins
3. Run Jenkins in debug mode: java -jar jenkins.war --debug

DevOps Tools Integration

1. Docker: docker build, docker run, docker push
2. Git: git clone, git pull, git push
3. Maven: mvn clean package, mvn deploy
4. Ansible: ansible-playbook playbook.yml

Additional Resources

1. Jenkins CLI Documentation (Jenkins)
2. Jenkins Pipeline Documentation (Jenkins)
3. DevOps Tutorial (Tutorials Point)
4. Jenkins Troubleshooting Guide (Jenkins)
   

#### Jenkins Automation Commands
```
1. Restart Jenkins: sudo service jenkins restart
2. Stop Jenkins: sudo service jenkins stop
3. Start Jenkins: sudo service jenkins start
4. Check Jenkins status: sudo service jenkins status
5. Update Jenkins plugins: jenkins-cli update-plugin
6. Install Jenkins plugin: jenkins-cli install-plugin
7. Uninstall Jenkins plugin: jenkins-cli uninstall-plugin
8. List Jenkins plugins: jenkins-cli list-plugins
9. Check Jenkins logs: sudo less /var/log/jenkins/jenkins.log
10. Clear Jenkins workspace: jenkins-cli clean-workspace
```
#### Cron Job Automation Commands

```text
1. Open crontab editor: crontab -e
2. Add cron job: minute hour day month day_of_week command
3. List cron jobs: crontab -l
4. Remove cron job: crontab -r
5. Run cron job manually: run-parts /etc/cron.hourly
```
#### File Path Not Found Automation Commands
```text
1. Create directory: mkdir -p /path/to/directory
2. Change directory ownership: chown -R user:group /path/to/directory
3. Change directory permissions: chmod -R 755 /path/to/directory
4. Check file existence: test -f /path/to/file
5. Create symbolic link: ln -s /path/to/target /path/to/link
```

#### Jenkinsfile Automation Commands


1. Define pipeline: pipeline { ... }
2. Define stage: stage('Stage Name') { ... }
3. Define step: step('Step Name') { ... }
4. Use environment variables: env.VARIABLE_NAME
5. Use credentials: withCredentials([usernamePassword(...)]) { ... }
```
#### Script Automation Commands

```text
1. Run shell script: sh /path/to/script.sh
2. Run Python script: python /path/to/script.py
3. Run Groovy script: groovy /path/to/script.groovy
4. Run Maven command: mvn clean package
5. Run Docker command: docker build -t image_name
```
#### Troubleshooting Automation Commands
```text
1. Check system logs: dmesg | grep error
2. Check Jenkins logs: sudo less /var/log/jenkins/jenkins.log
3. Check disk space: df -h
4. Check memory usage: free -m
5. Check CPU usage: top
```

#### Tips and Tricks
```text
1. Use man command to learn about commands.
2. Use command --help for brief help.
3. Use Ctrl+C to cancel a command.
4. Use Ctrl+Z to background a command.
5. Use screen or tmux for multiple terminal sessions.
```

