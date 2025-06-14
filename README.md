# k8s-practice

## 一步一步來

1. 安裝MicroK8s（單機練習神器）

   - 基本安裝

       ```bash
       sudo snap install microk8s --classic
       sudo usermod -a -G microk8s $USER
       newgrp microk8s
       microk8s status --wait-ready
       ```

   - 開啟dns模組

       ```bash
       microk8s enable dns ingress
       ```

2. 準備 Go API 程式與 Docker 映像
3. 建 Docker 映像並上傳（假設用 Docker Hub）
4. 第四步：撰寫 Kubernetes YAML 檔
5. 部署應用
