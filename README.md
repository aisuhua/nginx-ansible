# Nginx Ansible

使用 Ansible 安装 Nginx

## 使用

```sh
git clone git@github.com:aisuhua/nginx-ansible.git
cd nginx-ansible

# 按需调整服务器 IP、安装目录等
vim hosts.yaml

ansible-playbook playbook.yaml
```

## 卸载

```sh
ansible-playbook remove.yaml
```

## 特点

- 支持在单机上安装多个 Nginx 实例
- 卸载简单，方便来回测试
- 默认安装了 [ngx_http_proxy_connect_module](https://github.com/chobits/ngx_http_proxy_connect_module) 和 [nginx-module-vts](https://github.com/vozlt/nginx-module-vts) 这两个非官方模块
