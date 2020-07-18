
## Details

Deploy any number of EC2 Sample flask web servers with  mysql  and Extra EC2 instanc which monitor all web servers.

## AWS credintials

* You can store them in ```.boto``` file
* Or export to the environment variable using ```export AWS_ACCESS_KEY=XXXXXXX  ``` and ```export AWS_SECRET_KEY=XXXXXXX``` **as of now this step is implemented in code** 
* Or you can directly declare them as variables, in ```group_vars``` or in ```playbook vars```.

> So modify    ```ec2_create``` role according to your usage

## Required

* You need to provide the git hub repo link where you flask application has present.
* make sure that there is a ```.sql``` file for ```Tables``` creation.
* The name of python file should be ```app.py```
* make Modification's to nagios also , you are free to add notification alerts.
* The default nagios credintials are:
    * user_name: nagiosadmin and password is password itslef.
* you cann add any name and password, and you can change monitoring thresholds.

* The code works for all linux Distributions like Ubuntu,CentOS, RedHat etc..,



> Your'e free to change the code and any contributions and suggestions are welcomed.

## References

* sample flask application is from [here](https://github.com/EswarGitHub/GymManagementSystem) where i have modified and fixed some errors, the updatd version is [here](https://github.com/saireddyavs/Gym-appication).
* for monitoring i used help from [Sam-Darwins repo](https://github.com/sdarwin/Ansible-Nagios). 
