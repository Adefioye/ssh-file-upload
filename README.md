# Using Paramiko SSH & SCP to Upload Files to Remote Server

This repo is primarily based on the [article](https://hackersandslackers.com/automate-ssh-scp-python-paramiko/)


## Getting Started


### Installation

```shell
$ sudo apt install make
$ git clone https://github.com/Adefioye/ssh-file-upload.git
$ cd ssh-file-upload
$ sudo apt-get install python3.7-venv
$ python3 -m venv venv
$ source venv/bin/activate
$ make install
$ make run
```

### Configuration

Replace the values in **.env** with your values.

* `ENVIRONMENT`: Contextual environment the script is being on.
* `SSH_REMOTE_HOST`: IP address (or URL) of remote host to SSH into.
* `SSH_USERNAME`: Username for connecting to remote host.
* `SSH_PASSWORD` _(optional)_: Password of user SSHing into remote host via basic auth.
* `SSH_KEY_FILEPATH`: /path/to/local/sshkey
* `SCP_DESTINATION_FOLDER` _(optional)_: Remote directory to serve as destination for file uploads.

*Remember to never commit secrets saved in .env files to Github.*

-----

<!-- **Hackers and Slackers** tutorials are free of charge. If you found this tutorial helpful, a [small donation](https://www.buymeacoffee.com/hackersslackers) would be greatly appreciated to keep us in business. All proceeds go towards coffee, and all coffee goes towards more content. -->


