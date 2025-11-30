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
ansible-playbook zeekbuild.yaml -vv
```

