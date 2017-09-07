情報共有
--
# simpleブランチ

簡易playbook

```
git checkout simple
ansible-playbook -i test_hosts modules.yml -k -K
```

# branch1

roles分離

```
git checkout branch1
ansible-playbook -i test_hosts site.yml -k -K
```
