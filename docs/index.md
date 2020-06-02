# TheHive4py

TheHive4py is a Python API client for [TheHive](https://thehive-project.org/), a scalable 3-in-1 open source and free security incident response platform designed to make life easier for SOCs, CSIRTs, CERTs and any information security practitioner dealing with security incidents that need to be investigated and acted upon swiftly.

TheHive4py allows analysts to send alerts to TheHive out of different sources. Those alerts can then be previewed and imported into cases using pre-defined templates.

For example, a SOC may ask its constituency to send suspicious email reports to a specific mailbox that a script polls at regular intervals. When a new email is received, the script parses it then calls TheHive4py to create a corresponding alert in TheHive. Once the alert is raised, SOC analysts will get a notification thanks to TheHive's live stream so they can preview it and import it if deemed worth investigating using a specific template.

## Features

TheHive4py allows the following features:

=== "Authentication"
    - [X] [Using and API key](reference/auth#thehive4py.auth.BearerAuth)
    - [X] [Using a username/password pair](reference/auth#thehive4py.auth.BasicAuth)
=== "Alerts"
    - [X] [Search for alerts](reference/api#thehive4py.api.TheHiveApi.find_alerts)
    - [X] [Create alert](reference/api#thehive4py.api.TheHiveApi.create_alert)
    - [X] [Update alert](reference/api#thehive4py.api.TheHiveApi.update_alert)
    - [ ] Delete alert
=== "Cases"
    - [X] [Search for cases](reference/api#thehive4py.api.TheHiveApi.find_cases)
    - [X] [Create case](reference/api#thehive4py.api.TheHiveApi.create_case)
    - [X] [Update case](reference/api#thehive4py.api.TheHiveApi.update_case)
    - [X] [Delete case](reference/api#thehive4py.api.TheHiveApi.delete_case)
    - [X] [Get related cases](reference/api#thehive4py.api.TheHiveApi.get_linked_case)
=== "Tasks"
    - [X] Search for tasks
    - [X] Create and update tasks
    - [X] Delete tasks
    - [X] Create task log
    - [ ] Run responder on task
=== "Observables"
    - [X] Search for observables
    - [X] Create observable
    - [X] Update observable
    - [ ] Delete observable
    - [X] Run analyzer on observable
    - [ ] Run responder on observable

=== "Administration"
    - [X] [Search for Case templates](reference/api#thehive4py.api.find_case_templates)
    - [X] [Get Case template by name](reference/api#thehive4py.api.get_case_template)
    - [X] [Create Case templates](reference/api#thehive4py.api.create_case_template)
    - [ ] Create custom fields


## Installation

On macOS and Linux, type:

```bash
sudo pip install thehive4py
```

If you are using Python on a Windows operating system, please forgo the `sudo` command.

## License
TheHive4py is an open source and free software released under the [AGPL](https://github.com/TheHive-Project/TheHive/blob/master/LICENSE) (Affero General Public License). We, TheHive Project, are committed to ensure that TheHive4py will remain a free and open source project on the long-run.


## Updates
Information, news and updates are regularly posted on [TheHive Project Twitter account](https://twitter.com/thehive_project) and on [the blog](https://blog.thehive-project.org/).


## Contributing
We welcome your contributions. Please feel free to fork the code, play with it, make some patches and send us pull requests using [issues](https://github.com/TheHive-Project/TheHive4py/issues).

We do have a [Code of conduct](code_of_conduct.md). Make sure to check it out before contributing.


## Support
Please [open an issue on GitHub](https://github.com/TheHive-Project/TheHive4py/issues/new) if you'd like to report a bug or request a feature. We are also available on [Gitter](https://gitter.im/TheHive-Project/TheHive) to help you out.

If you need to contact the project team, send an email to <support@thehive-project.org>.


## Community Discussions
We have set up a Google forum at <https://groups.google.com/a/thehive-project.org/d/forum/users>. To request access, you need a Google account. You may create one [using a Gmail address](https://accounts.google.com/SignUp?hl=en) or [without one](https://accounts.google.com/SignUpWithoutGmail?hl=en).


## Website
<https://thehive-project.org/>