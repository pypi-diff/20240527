# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.27a1716702262.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.28a1716765099.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.27a1716702262.tar", last modified: Sun May 26 05:46:52 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.28a1716765099.tar", last modified: Sun May 26 23:14:21 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262.tar` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.778846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 05:46:52.778846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.762846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     5051 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.766846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      864 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    39619 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9584 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5740 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4399 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4531 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     3065 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2560 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2860 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8791 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4826 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5799 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23901 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12558 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    56778 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.770846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1193 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1767 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    26794 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    14674 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
--rw-------   0 runner    (1001) docker     (127)    39093 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/control_plane_node.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)    13465 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    25513 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5199 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
--rw-------   0 runner    (1001) docker     (127)     5115 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     5187 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
--rw-------   0 runner    (1001) docker     (127)     5157 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
--rw-------   0 runner    (1001) docker     (127)    43829 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/worker_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.774846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.774846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      570 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     2920 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    61362 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    52391 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:46:52.778846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 05:46:52.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-26 05:46:52.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 05:46:52.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-26 05:46:52.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 05:46:52.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-26 05:46:45.000000 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 05:46:52.778846 pulumi_kubernetes_the_hard_way-0.0.27a1716702262/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.856382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 23:14:21.856382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.840382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     5131 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.844382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      864 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    39619 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9584 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5740 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4399 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4531 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     3065 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2560 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2860 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5799 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    56778 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.848382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1230 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1767 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    26794 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14674 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
+-rw-------   0 runner    (1001) docker     (127)    39093 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/control_plane_node.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)    13465 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    25513 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5199 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
+-rw-------   0 runner    (1001) docker     (127)     5115 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     5187 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
+-rw-------   0 runner    (1001) docker     (127)     5157 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+-rw-------   0 runner    (1001) docker     (127)    43829 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/worker_node.py
+-rw-------   0 runner    (1001) docker     (127)     6692 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/worker_pre_requisites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.852382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.856382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      570 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     2920 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    61362 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    15125 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15217 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15357 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    15125 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    15160 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    15020 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    52391 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    15020 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    15055 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15287 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    15055 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    15075 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    15090 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:14:21.856382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 23:14:21.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-26 23:14:21.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:14:21.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-26 23:14:21.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 23:14:21.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-26 23:14:12.000000 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:14:21.856382 pulumi_kubernetes_the_hard_way-0.0.28a1716765099/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.27a1716702262
+Version: 0.0.28a1716765099
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/README.md` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartContainerd": "StartContainerd",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StartKubeProxy": "StartKubeProxy",
    "kubernetes-the-hard-way:remote:StartKubelet": "StartKubelet",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService",
-   "kubernetes-the-hard-way:remote:WorkerNode": "WorkerNode"
+   "kubernetes-the-hard-way:remote:WorkerNode": "WorkerNode",
+   "kubernetes-the-hard-way:remote:WorkerPreRequisites": "WorkerPreRequisites"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
   "fqn": "pulumi_kubernetes_the_hard_way.tls",
   "classes": {
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 from .start_containerd import *
 from .start_etcd import *
 from .start_kube_proxy import *
 from .start_kubelet import *
 from .static_pod import *
 from .systemd_service import *
 from .worker_node import *
+from .worker_pre_requisites import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/containerd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/containerd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/control_plane_node.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/control_plane_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_containerd.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_containerd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/remote/worker_node.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/remote/worker_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -131,15 +131,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -182,15 +182,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -132,15 +132,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -183,15 +183,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -330,15 +330,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -132,15 +132,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -183,15 +183,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -330,15 +330,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['MkdirArgs', 'Mkdir']
+__all__ = ['MktempArgs', 'Mktemp']
 
 @pulumi.input_type
-class MkdirArgs:
+class MktempArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Mkdir resource.
+        The set of arguments for constructing a Mktemp resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -131,129 +131,129 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Mkdir(pulumi.ComponentResource):
+class Mktemp(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `mkdir` utility on a remote system.
+        Abstraction over the `mktemp` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MkdirArgs,
+                 args: MktempArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `mkdir` utility on a remote system.
+        Abstraction over the `mktemp` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MkdirArgs args: The arguments to use to populate this resource's properties.
+        :param MktempArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MktempArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MkdirArgs.__new__(MkdirArgs)
+            __props__ = MktempArgs.__new__(MktempArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mkdir, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mkdir',
+        super(Mktemp, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mktemp',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['MktempArgs', 'Mktemp']
+__all__ = ['TeeArgs', 'Tee']
 
 @pulumi.input_type
-class MktempArgs:
+class TeeArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Mktemp resource.
+        The set of arguments for constructing a Tee resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -131,129 +132,129 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Mktemp(pulumi.ComponentResource):
+class Tee(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `mktemp` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MktempArgs,
+                 args: TeeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `mktemp` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MktempArgs args: The arguments to use to populate this resource's properties.
+        :param TeeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MktempArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MktempArgs.__new__(MktempArgs)
+            __props__ = TeeArgs.__new__(TeeArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mktemp, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mktemp',
+        super(Tee, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tee',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -329,15 +330,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['MvArgs', 'Mv']
+__all__ = ['MkdirArgs', 'Mkdir']
 
 @pulumi.input_type
-class MvArgs:
+class MkdirArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Mv resource.
+        The set of arguments for constructing a Mkdir resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -131,129 +131,129 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Mv(pulumi.ComponentResource):
+class Mkdir(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `mv` utility on a remote system.
+        Abstraction over the `mkdir` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MvArgs,
+                 args: MkdirArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `mv` utility on a remote system.
+        Abstraction over the `mkdir` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MvArgs args: The arguments to use to populate this resource's properties.
+        :param MkdirArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MvArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MvArgs.__new__(MvArgs)
+            __props__ = MkdirArgs.__new__(MkdirArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mv, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mv',
+        super(Mkdir, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mkdir',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -131,15 +131,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -182,15 +182,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -131,15 +131,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -182,15 +182,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -132,15 +132,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -183,15 +183,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -330,15 +330,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
@@ -131,15 +131,15 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
@@ -182,15 +182,15 @@
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] create: The command to run on create.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
         :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['TeeArgs', 'Tee']
+__all__ = ['WgetArgs', 'Wget']
 
 @pulumi.input_type
-class TeeArgs:
+class WgetArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Tee resource.
+        The set of arguments for constructing a Wget resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -132,129 +131,129 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Tee(pulumi.ComponentResource):
+class Wget(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TeeArgs,
+                 args: WgetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TeeArgs args: The arguments to use to populate this resource's properties.
+        :param WgetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TeeArgs.__new__(TeeArgs)
+            __props__ = WgetArgs.__new__(WgetArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tee, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tee',
+        super(Wget, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Wget',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -330,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['WgetArgs', 'Wget']
+__all__ = ['MvArgs', 'Mv']
 
 @pulumi.input_type
-class WgetArgs:
+class MvArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Wget resource.
+        The set of arguments for constructing a Mv resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -131,129 +131,129 @@
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Wget(pulumi.ComponentResource):
+class Mv(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `mv` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] create: The command to run on create.
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] update: The command to run on update, if empty, create will 
+        :param pulumi.Input[Sequence[Any]] triggers: Trigger replacements on changes to this input.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: WgetArgs,
+                 args: MvArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `mv` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param WgetArgs args: The arguments to use to populate this resource's properties.
+        :param MvArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MvArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
-                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = WgetArgs.__new__(WgetArgs)
+            __props__ = MvArgs.__new__(MvArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Wget, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Wget',
+        super(Mv, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mv',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -329,15 +329,15 @@
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        TODO
+        Trigger replacements on changes to this input.
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
     def update(self) -> pulumi.Output[Optional[Any]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.27a1716702262
+Version: 0.0.28a1716765099
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 pulumi_kubernetes_the_hard_way/remote/start_containerd.py
 pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
 pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/remote/worker_node.py
+pulumi_kubernetes_the_hard_way/remote/worker_pre_requisites.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
 pulumi_kubernetes_the_hard_way/tls/outputs.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.27a1716702262/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.28a1716765099/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.12.0,<5.0.0", "pulumi-random>=4.16.2,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.27a1716702262"
+  version = "0.0.28a1716765099"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

