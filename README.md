- name: Install expect
  package:
    name: expect
    state: present

- name: test connection to TSM Server
  shell: |
    expect -c '
      spawn dsmc q session
      expect "Password:"
      send "{{ tsm_password }}\r"
      expect eof
    '

