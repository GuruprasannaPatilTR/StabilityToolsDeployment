# StabilityToolsDeployment

Above files are already in deployment server. Any changes in the code will be updated. If it is not present you can alway use this GIT repository for downloading ZIP file or Clone it.

# Usage:

- Login to c129hdb.int.thomsonreuters with your M account and become root user.
- cd /appserver/Stability_Tools.
- Various Use case based on the Environment and Tools are as below.

# Client:

**IMPORTANT:** Make sure you are Using this for **CLIENT**.


  **Novus Audit**
  - ansible-playbook playbook-NovusAudit.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Client"
  - **Ex:** ansible-playbook playbook-NovusAudit.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Client"
  
  **Novus-content-restore**
  - ansible-playbook playbook-NovusContentRestore.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Client"
  - **Ex:** ansible-playbook playbook-NovusContentRestore.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Client"
  
  **NovusCCIRestore**
  - ansible-playbook playbook-NovusCCIRestore.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Client"
  - **Ex:** ansible-playbook playbook-NovusCCIRestore.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Client"

# Prod:

**IMPORTANT:** Make sure you are Using this for **PROD**.


**Novus Audit**
  - ansible-playbook playbook-NovusAudit.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Prod"
  - **Ex:** ansible-playbook playbook-NovusAudit.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Prod"
  
  **Novus-content-restore**
  - ansible-playbook playbook-NovusContentRestore.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Prod"
  - **Ex:** ansible-playbook playbook-NovusContentRestore.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Prod"
  
  **NovusCCIRestore**
  - ansible-playbook playbook-NovusCCIRestore.yml -i StabilityTools_hosts --extra-vars "old_version=\*.\*.\*.\* new_version=\*.\*.\*.\* hosts=StabilityTools_Prod"
  - **Ex:** ansible-playbook playbook-NovusCCIRestore.yml -i StabilityTools_hosts --extra-vars "old_version=19.6.0.1 new_version=21.14.0.12 hosts=StabilityTools_Prod"
 
  

