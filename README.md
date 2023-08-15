# inert
透過Ansible快速搭建環境,通過`ansible/group_vars/all.yaml`聲明對應服務和目標機器IP。
- 可以安裝哪些服務：
 - docker
 - k8s
 - nfs
 - drdb
 - GoCD
---
## 使用步驟
1. git clone專案
    ```bash
        cd $HOME
        git clone 
    ```

2. 安裝docker
    ```bash
        bash inert/ubuntu22/scripts/docker_install.sh
    ```

3. 設定cmd
    ```bash
        sudo cp inert/ubuntu22/bin/inert-local /bin/inert
    ```
4. 啟動inert，第一次執行時會構建image，構建完後，只要輸入`inert`就會進入操作環境。