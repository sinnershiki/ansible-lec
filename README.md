情報共有
--
# branch0

簡易playbook

```
git checkout branch0
ansible-playbook -i test_hosts site.yml -k -K
```

# branch1

roles分離

```
git checkout branch1
ansible-playbook -i test_hosts site.yml -k -K
```

# branch2

notify

```
git checkout branch2
ansible-playbook -i test_hosts site.yml -k -K
```

# branch3

tags

```
git checkout branch3
ansible-playbook -i test_hosts site.yml -k -K --tags "user"
```

# branch4

本番、ステージング分離

```
git checkout branch4
ansible-playbook -i test_hosts site.yml -k -K --tags "ansible, nginx"
```
