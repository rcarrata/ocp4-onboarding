# LafargeHolcim Onboarding Automation Project

This project is created for the automation of the onboarding of projects, apps, etc.

## Usage:

* Clone this repository.

* Log on to an OpenShift server oc login -u <user> https://<server>:<port>/

* Install the required openshift-applier dependency:

```
ansible-galaxy install -r requirements.yml --roles-path=roles
```

Run the play book using this to create projects and roles

ansible-playbook apply.yml -i inventory/ -e target=tools

```
ansible-playbook apply.yml -e target=request   -i inventory/   -e skip_version_checks=true
```
