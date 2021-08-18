## 참고
* https://www.lainyzine.com/ko/article/creating-ssh-key-for-github/

## ssh-keygen
  ```
  ssh-keygen -t ed25519 -C "your_email@example.com"
  ```
  or
  ```
  ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
  ```

## ~/.ssh/config
  ```
  Host github.com
    IdentityFile ~/.ssh/id_ed25519
    User git
  ```

## test
* ssh -T git@github.com


