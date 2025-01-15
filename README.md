![Github Watchers](https://badgen.net/github/watchers/openwrtbuild/Url-Shorten-Worker)![Github Stars](https://badgen.net/github/stars/openwrtbuild/Url-Shorten-Worker)![Github Forks](https://badgen.net/github/forks/openwrtbuild/Url-Shorten-Worker)

# Url-Shorten-Worker
A URL Shortener created using Cloudflare Worker

# API

[API Documentation](docs/API.md)[API文档](docs/API_zh-hans.md))

# Getting start
### 去Workers KV中创建一个命名空间

Go to Workers KV and create a namespace.

![](docs/kv_create_namespace.png)

### 去Worker的Settings选项卡中绑定KV Namespace

Bind an instance of a KV Namespace to access its data in a Worker.

![](docs/worker_settings.jpg)

### 其中Variable name填写`LINKS`, KV namespace 选择你刚刚创建的命名空间

Where Variable name should set as `LINKS` and KV namespace is the namespace you just created in the first step.

![](docs/worker_kv_binding.png)

### 并入AoEiuV020/Url-Shorten-Worker [repo](https://github.com/AoEiuV020/Url-Shorten-Worker)的功能，配置其他环境变量参考此仓库说明（例如WHITE_LIST, PASSWORD, DEFAULT_LEN, SHORTEN_TIMEOUT）。

Merge some functions from AoEiuV020/Url-Shorten-Worker [repo](https://github.com/AoEiuV020/Url-Shorten-Worker). Refer to the variable configuration (e.g. WHITE_LIST, PASSWORD, DEFAULT_LEN, SHORTEN_TIMEOUT).

### 复制本项目中的`index.js`的代码到Cloudflare Worker 

Copy the `index.js` code from this project to Cloudflare Worker. 

### 点击Save and Deploy

Click Save and Deploy

