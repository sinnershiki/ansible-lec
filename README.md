情報共有
--
# branch4

本番、ステージング分離

```
git checkout branch4
ansible-playbook -i test_hosts site.yml -k -K --tags "ansible, nginx"
```
