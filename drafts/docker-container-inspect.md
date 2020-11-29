# docker container inspect

[「沈黙は金なり」Unixの哲学](https://ja.wikipedia.org/wiki/UNIX%E5%93%B2%E5%AD%A6)
あえてアウトプットするのは、出力されるメッセージが金以上の価値がある。

データー構造を紐解くことで、コンテナーを知れるだろう。

```shell
➜  re-using-docker git:(master) bash -c 'docker inspect $(docker ps -q)'
[
    {
        "Id": "0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd",
        "Created": "2019-01-30T03:59:32.814783033Z",
        "Path": "/cmd.sh",
        "Args": [],
        "State": {
            "Status": "running",
            "Running": true,
            "Paused": false,
            "Restarting": false,
            "OOMKilled": false,
            "Dead": false,
            "Pid": 2393,
            "ExitCode": 0,
            "Error": "",
            "StartedAt": "2019-01-30T03:59:33.538422139Z",
            "FinishedAt": "0001-01-01T00:00:00Z"
        },
        "Image": "sha256:bb9a3caa442f754c05a3bd9d14cb833a6ee9e7902e849e001b281038da4f9b55",
        "ResolvConfPath": "/var/lib/docker/containers/0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd/resolv.conf",
        "HostnamePath": "/var/lib/docker/containers/0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd/hostname",
        "HostsPath": "/var/lib/docker/containers/0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd/hosts",
        "LogPath": "/var/lib/docker/containers/0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd/0730bf4359f6409b1c89a550200aa37b02f7f03e7282357c0db74036a55fa2fd-json.log",
        "Name": "/eloquent_dhawan",
        "RestartCount": 0,
        "Driver": "overlay2",
        "Platform": "linux",
        "MountLabel": "",
        "ProcessLabel": "",
        "AppArmorProfile": "",
        "ExecIDs": null,
        "HostConfig": {
            "Binds": null,
            "ContainerIDFile": "",
            "LogConfig": {
                "Type": "json-file",
                "Config": {}
            },
            "NetworkMode": "default",
            "PortBindings": {
                "5000/tcp": [
                    {
                        "HostIp": "",
                        "HostPort": "5000"
                    }
                ]
            },
            "RestartPolicy": {
                "Name": "no",
                "MaximumRetryCount": 0
            },
            "AutoRemove": false,
            "VolumeDriver": "",
            "VolumesFrom": null,
            "CapAdd": null,
            "CapDrop": null,
            "Dns": [],
            "DnsOptions": [],
            "DnsSearch": [],
            "ExtraHosts": null,
            "GroupAdd": null,
            "IpcMode": "shareable",
            "Cgroup": "",
            "Links": null,
            "OomScoreAdj": 0,
            "PidMode": "",
            "Privileged": false,
            "PublishAllPorts": false,
            "ReadonlyRootfs": false,
            "SecurityOpt": null,
            "UTSMode": "",
            "UsernsMode": "",
            "ShmSize": 67108864,
            "Runtime": "runc",
            "ConsoleSize": [
                0,
                0
            ],
            "Isolation": "",
            "CpuShares": 0,
            "Memory": 0,
            "NanoCpus": 0,
            "CgroupParent": "",
            "BlkioWeight": 0,
            "BlkioWeightDevice": [],
            "BlkioDeviceReadBps": null,
            "BlkioDeviceWriteBps": null,
            "BlkioDeviceReadIOps": null,
            "BlkioDeviceWriteIOps": null,
            "CpuPeriod": 0,
            "CpuQuota": 0,
            "CpuRealtimePeriod": 0,
            "CpuRealtimeRuntime": 0,
            "CpusetCpus": "",
            "CpusetMems": "",
            "Devices": [],
            "DeviceCgroupRules": null,
            "DiskQuota": 0,
            "KernelMemory": 0,
            "MemoryReservation": 0,
            "MemorySwap": 0,
            "MemorySwappiness": null,
            "OomKillDisable": false,
            "PidsLimit": 0,
            "Ulimits": null,
            "CpuCount": 0,
            "CpuPercent": 0,
            "IOMaximumIOps": 0,
            "IOMaximumBandwidth": 0,
            "MaskedPaths": [
                "/proc/asound",
                "/proc/acpi",
                "/proc/kcore",
                "/proc/keys",
                "/proc/latency_stats",
                "/proc/timer_list",
                "/proc/timer_stats",
                "/proc/sched_debug",
                "/proc/scsi",
                "/sys/firmware"
            ],
            "ReadonlyPaths": [
                "/proc/bus",
                "/proc/fs",
                "/proc/irq",
                "/proc/sys",
                "/proc/sysrq-trigger"
            ]
        },
        "GraphDriver": {
            "Data": {
                "LowerDir": "/var/lib/docker/overlay2/759e4d47be583e48d4fd123f4e0351f933583a19894fb8ba45288f53d478ad2c-init/diff:/var/lib/docker/overlay2/0acf718266cbedcbebd53970433cb9a9deeddc2fb596520f6311902678c5780d/diff:/var/lib/docker/overlay2/a575e15380823c54a29d25d9cc9a678387c2c870a8e52de374ab2b3df7bda4b3/diff:/var/lib/docker/overlay2/a3c366b254d82864ad1bce0c7c4d4682e1c341d33a6721739cd82cbda7e6947f/diff:/var/lib/docker/overlay2/bd9616ec21c749464fb488855b68fdb33e4db726847c6688ec9b2861b85dbf2f/diff:/var/lib/docker/overlay2/08fa7f206ab2a2c4f3136b642834525b675c1588121051684eff5dc8db147854/diff:/var/lib/docker/overlay2/3c8d95a4b1cf3f8fa7a79ce24fb4d64c3a717c7b438e8803ddbca448e5cd7bd1/diff:/var/lib/docker/overlay2/121b47138acca247041305f4d6fc6adaa51de37b38f729a6811bf6cdc434c7a8/diff:/var/lib/docker/overlay2/ab1426abff34100404fd021d34e4d47b647047c764cf48aa45c177e5dbc79f8a/diff:/var/lib/docker/overlay2/04c759a4202b010ad9cf64b25603b330f31017d42ac3c6b1cc143d99d8ae2d36/diff:/var/lib/docker/overlay2/eab2e19aa3f6bf47d9c359f66bc894861f785a33efaecddb27e016c1652119ba/diff:/var/lib/docker/overlay2/628884b003fa3bccd4b8e41cd7394081261a1118ee89630a5aec901cca44dc07/diff:/var/lib/docker/overlay2/4dc60fb000bfaf959831fbb4f789e7afaaadfd210acd9863638efd5b912cfc28/diff:/var/lib/docker/overlay2/a54db225d7bbda1e85a4b25f7a713a5b939325c21d4cebddcdb095d37d912362/diff:/var/lib/docker/overlay2/ec186ae23d2ae6481bf3d7d7f4e19d7fc77c27e29a6b4032fb59d17529f451ca/diff",
                "MergedDir": "/var/lib/docker/overlay2/759e4d47be583e48d4fd123f4e0351f933583a19894fb8ba45288f53d478ad2c/merged",
                "UpperDir": "/var/lib/docker/overlay2/759e4d47be583e48d4fd123f4e0351f933583a19894fb8ba45288f53d478ad2c/diff",
                "WorkDir": "/var/lib/docker/overlay2/759e4d47be583e48d4fd123f4e0351f933583a19894fb8ba45288f53d478ad2c/work"
            },
            "Name": "overlay2"
        },
        "Mounts": [],
        "Config": {
            "Hostname": "0730bf4359f6",
            "Domainname": "",
            "User": "uwsgi",
            "AttachStdin": false,
            "AttachStdout": false,
            "AttachStderr": false,
            "ExposedPorts": {
                "5000/tcp": {},
                "9090/tcp": {},
                "9191/tcp": {}
            },
            "Tty": false,
            "OpenStdin": false,
            "StdinOnce": false,
            "Env": [
                "PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin",
                "LANG=C.UTF-8",
                "GPG_KEY=97FC712E4C024BBEA48A61ED3A5CA953F73C700D",
                "PYTHON_VERSION=3.4.9",
                "PYTHON_PIP_VERSION=19.0.1"
            ],
            "Cmd": [
                "/cmd.sh"
            ],
            "ArgsEscaped": true,
            "Image": "identidock",
            "Volumes": null,
            "WorkingDir": "/app",
            "Entrypoint": null,
            "OnBuild": null,
            "Labels": {}
        },
        "NetworkSettings": {
            "Bridge": "",
            "SandboxID": "0caf81213e51a555960a2faf94b08b0c26a9873950dda6de8dd7b465d1237374",
            "HairpinMode": false,
            "LinkLocalIPv6Address": "",
            "LinkLocalIPv6PrefixLen": 0,
            "Ports": {
                "5000/tcp": [
                    {
                        "HostIp": "0.0.0.0",
                        "HostPort": "5000"
                    }
                ],
                "9090/tcp": null,
                "9191/tcp": null
            },
            "SandboxKey": "/var/run/docker/netns/0caf81213e51",
            "SecondaryIPAddresses": null,
            "SecondaryIPv6Addresses": null,
            "EndpointID": "ec4c56cd1c6e7048b446f74439cefef933ba9d06c48a54f88c5ef60400aed38a",
            "Gateway": "172.17.0.1",
            "GlobalIPv6Address": "",
            "GlobalIPv6PrefixLen": 0,
            "IPAddress": "172.17.0.2",
            "IPPrefixLen": 16,
            "IPv6Gateway": "",
            "MacAddress": "02:42:ac:11:00:02",
            "Networks": {
                "bridge": {
                    "IPAMConfig": null,
                    "Links": null,
                    "Aliases": null,
                    "NetworkID": "f6ef9e6fa32183b83d6664fd81ae507be9dde86d7fc112c0b303a8ac122af76f",
                    "EndpointID": "ec4c56cd1c6e7048b446f74439cefef933ba9d06c48a54f88c5ef60400aed38a",
                    "Gateway": "172.17.0.1",
                    "IPAddress": "172.17.0.2",
                    "IPPrefixLen": 16,
                    "IPv6Gateway": "",
                    "GlobalIPv6Address": "",
                    "GlobalIPv6PrefixLen": 0,
                    "MacAddress": "02:42:ac:11:00:02",
                    "DriverOpts": null
                }
            }
        }
    }
]
➜  re-using-docker git:(master)
```