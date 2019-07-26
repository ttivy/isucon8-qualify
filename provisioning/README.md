# torb provisioning

python実装のみdeploy

```sh
# GCP で isucon ユーザーのssh鍵を設定しておく
$ vim hosts
# host を設定
$ ansible-playbook -i hosts site.yml --skip-tags "create_user"


# isucon ユーザーが既に存在しない場合
$ vim hosts
# host 及び ssh_user を設定
$ ansible-playbook -i hosts site.yml
```
