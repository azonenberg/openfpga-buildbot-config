# openfpga-buildbot-config

To provision a VM from scratch:

  * Configure `hosts.cfg`;
  * Configure `vars/secrets.yml` (see `vars/secrets.yml.sample`);
  * Run `ansible-playbook buildserver.yaml`.

To bring VM configuration up to date:

  * Run `ansible-playbook buildserver.yaml`.

To update buildmaster configuration only:

  * Run `ansible-playbook buildserver.yaml --tags buildmaster-config`.
