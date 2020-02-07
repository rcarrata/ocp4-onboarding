# LafargeHolcim Onboarding Automation Project

This project is created for the automation of the onboarding of projects, apps, etc.

## Usage:

* Clone this repository.

* Log on to an OpenShift server oc login -u <user> https://<server>:<port>/

* Install the required openshift-applier dependency:

```
ansible-galaxy install -r requirements.yml --roles-path=roles
```

* Run the play book using this to create projects and roles

```
ansible-playbook new_project.yml -e size=medium -e namespace_prefix=testing -i inventory/ -e skip_version_checks=true
```
