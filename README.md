# Upgrade Java from 11 to 17 using Ansible

Provide 600 permission on private key  testkey.pem using the command **chmod 600 testkey.pem** 

![image](https://github.com/user-attachments/assets/9d4708eb-4cb7-4f2c-b882-71338b28ea2c)

Command to run ansible-playbook is shown below
![image](https://github.com/user-attachments/assets/028e0eec-0837-499d-beb1-648d4279ce0e)
<br><br/>
java version, JAVA_HOME and PATH before and after the Java Upgrade is shown in Screenshots below.

**Before Java Upgrade on Amazon Linux2**
![image](https://github.com/user-attachments/assets/67887416-f63d-470b-9288-c9d8e2724aa0)

**After Java Upgrade on Amazon Linux2**
![image](https://github.com/user-attachments/assets/fb28bb15-7ba1-4e17-9c8d-26c7507f42e5)

**Before Java Upgrade on Rocky Linux**
![image](https://github.com/user-attachments/assets/c5597b32-101c-42f7-a265-791748ba4ae6)

**After Java Upgrade on Rocky Linux**
![image](https://github.com/user-attachments/assets/0e5243f7-3937-4328-95f2-dacc78430735)

**Before Java Upgrade on Alma Linux**
![image](https://github.com/user-attachments/assets/cb409912-35bd-4af5-9fa6-4b02905a5a51)

**After Java Upgrade on Alma Linux**
![image](https://github.com/user-attachments/assets/dd090a28-6fc8-4dee-99a7-7084191b5989)

**Before Java Upgrade on RHEL8**
![image](https://github.com/user-attachments/assets/6fb847a3-9f12-4261-a901-daf019f9e092)

**After Java Upgrade on RHEL8**
![image](https://github.com/user-attachments/assets/b2df0893-6883-4d01-9359-a580926f0aa6)

![image](https://github.com/user-attachments/assets/6d3f7f09-bd66-43d7-9e1f-1228eceaf772)

**Before Java Upgrade on Ubuntu**
![image](https://github.com/user-attachments/assets/a63345c3-a353-494d-9471-a0c111f8c09f)

**After Java Upgrade on Ubuntu**
![image](https://github.com/user-attachments/assets/fdad6311-7155-405a-98cd-db0e8e12ffd8)
<br><br/>
<br><br/>
<br><br/>
command to know the ansible_os_family, ansible_distribution etc.
```
ansible -i ./inventory/hosts -u ritesh --private-key testkey.pem -m setup | grep -i "ansible_os_family
ansible 52.170.102.16 -i ./inventory/hosts -u ritesh --private-key testkey.pem -m setup | grep -i "ansible_distribution"
```
