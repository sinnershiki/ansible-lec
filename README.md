情報共有
--
# simpleブランチ

簡易playbook

```
git checkout simple
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

# branch3 (masterは、現在この状態にREADMEが変更されている)

tags

```
git checkout branch3
ansible-playbook -i test_hosts site.yml -k -K --tags "user"
```
