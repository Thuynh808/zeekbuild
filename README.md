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

```bash
ansible-playbook _____.yaml -vv
```

- **sdfjklsdfjk**

```bash
ansible-playbook _____.yaml -vv
```

