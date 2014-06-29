# camlistore-ansible

An [ansible]() playbook for setting up a [camlistore]() server.

The server will have basic authentication and will serve over https.

## Usage

Create an inventory file with `username` and `password` variables set. These
will be used as your camlistore credentials.

For example:
```ini
[camlistore]
0.0.0.0 username=joeblogs password=supersecret
```

Then you can run the playbook.

```
pip install -r requirements.txt
ansible-playbook camlistore.yml -i hosts.ini
```
