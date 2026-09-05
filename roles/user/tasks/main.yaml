- name: app setup
  ansible.builtin.import_role:
    name: common
    tasks_from: app-setup.yaml

- name: nodejs setup
  ansible.builtin.import_role:
    name: common
    tasks_from: nodejs-setup.yaml

- name: systemd setup
  ansible.builtin.import_role:
    name: common
    tasks_from: systemd-setup.yaml

- name: start user
  ansible.builtin.service:
    name: user
    state: restarted
    enabled: yes