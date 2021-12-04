# 一个基于[monitor_docker](https://github.com/ualex73/monitor_docker)的容器监视卡片

### 本卡片说明：

* 本来是自己使用的，hassbian有人询问，所以就分享一下。
* 一切docker信息来源于集成 [monitor_docker](https://github.com/ualex73/monitor_docker)，该集成配置比较玄学，自己琢磨，勿cue。
* 源代码不是本人所有，原作者未发布成插件形式，我只是整理、部分内容汉化而已，感谢原作者！
* 整合之前已经在原作者GitHub相关代码提出issue，请求使用和修改。（目前回复允许使用和更改）。

### 版本说明：

###### V0.0.1

* 部分内容汉化，第一次同步到GitHub。

###### V0.0.2

* 加入卡片原作者地址，感谢原作者的代码。[原作者](https://github.com/bacco007)

# 使用方法：

预览：

<img src="https://raw.githubusercontent.com/Tao173/docker-card/main/docker.png" >

配置代码：

```
type: horizontal-stack
cards:
  - type: custom:stack-in-card
    cards:
      - type: custom:docker-card
        logo: /local/systemicons/mpd.png
        entitypart: docker_addon_243ffc37_mpd
      - type: custom:docker-card
        logo: /local/systemicons/mosquitto.png
        entitypart: docker_addon_core_mosquitto
  - type: custom:stack-in-card
    cards:
      - type: custom:docker-card
        logo: /local/systemicons/docker.png
        entitypart: docker_hassio_audio
      - type: custom:docker-card
        logo: /local/systemicons/docker.png
        entitypart: docker_hassio_cli
  - type: custom:stack-in-card
    cards:
      - type: custom:docker-card
        logo: /local/systemicons/docker.png
        entitypart: docker_hassio_observer
      - type: custom:docker-card
        logo: /local/systemicons/docker.png
        entitypart: docker_hassio_supervisor
  - type: custom:stack-in-card
    cards:
      - type: custom:docker-card
        logo: /local/systemicons/wangyiyun.png
        entitypart: docker_netease_cloud_music_api
      - type: custom:docker-card
        logo: /local/systemicons/qinglong.png
        entitypart: docker_qinglong

```

图标说明：

插件目录自带的有一部分图标，路径为/hacsfiles/docker-card/icons/

```
logo: /local/systemicons/docker.png
```

替换为：

```
logo: /hacsfiles/docker-card/icons/docker.png
```
