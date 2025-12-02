# ZeekBuild

- **Clone repo**

```bash
git clone -b build https://github.com/thuynh808/zeekbuild
cd zeekbuild
```

- **Configure inventory `hosts`**

```bash
vim inventory
```

- **Install collections**

```bash
./install_req.sh
```

- **Build Zeek**

```bash
ansible-playbook buildzeek.yaml -vv
```

- **Tune Zeek**

```bash
ansible-playbook tune-zeek.yaml -vv
```

- **Deploy ElasticSearch and Kibana Containers**

```bash
ansible-playbook deploy_elastic.yaml -vv
```

- **Configure Elastic/Kibana**

  - Enroll with token through UI
  - Run command on soc1 to retrieve verification code

```bash
docker exec -it kib01 bin/kibana-verification-code
```

- **Retrieve service token fleet server through UI**

  - Paste into `fleet_server.yaml` playbook

- **Deploy fleet server container **
```bash
ansible-playbook fleet_server.yaml -vv
```

