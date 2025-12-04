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

- **Sign in with elastic pw Elastic/Kibana**

- **Update pw for policy playbook**

```bash
vim policies_default.yaml
```

- **Create default policies and integrations for fleet server**

```bash
ansible-playbook policies_default.yaml -vv
```

- **Add fleet server through UI**

- **Add Agents through UI**
