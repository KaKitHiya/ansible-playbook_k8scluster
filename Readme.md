## 基于ansible_playbook实现了全自动安装部署kubernetes v1.32.1 + containerd集群，其中kubernetes组件和相关初始化镜像均修改为阿里云镜像代理，适合国内环境安装使用(containerd没有使用最新版，直接调用了docker的yum源安装)
## 集群分配三个角色，分别为master控制节点，worker工作节点，loadbalance负载均衡节点；其中负载均衡通过keepalived+nginx四层代理实现对api server的高可用
