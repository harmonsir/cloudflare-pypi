## PIP Fast Check 🛠️⚡

推荐使用 **`pip-fc`**！💯 这是提高开发效率的 **最佳选择**！✨ 一键自动配置，让你事半功倍！

🎉 **马上体验**：

> 安装指令：`pip install -U pip-fc` 🎶

👉 **[GitHub 介绍](https://github.com/harmonsir/pip-fc)** 👈 让你一步到位，快速了解所有功能！

如需要继续搭建mirror，请看下文介绍。

---

# Cloudflare-PyPI
利用Cloudflare反代，对PyPI.org源站进行国内加速。

## 为什么 /WHY
- 多一个PyPI镜像而已；而且域名短了更易记。
- 清华的镜像有时会出现某些包缺失的报错，而PyPI源站不会。

## 使用方法

- 临时使用
  >  `pip install -i https://pip.pylab.me some-package`

- 设为默认
  > `pip config set global.index-url https://pip.pylab.me/simple`

*反馈请提Issues*


## 更新

API内置`mappings`可以指定其他源， 譬如`https://pip.pylab.me/qh`，将会使用清华源。

```
mappings = {
  "/qh": "https://pypi.tuna.tsinghua.edu.cn/simple/",
  "/tuna": "https://pypi.tuna.tsinghua.edu.cn/simple/",
  "/hw": "https://repo.huaweicloud.com/repository/pypi/simple/",
  "/huawei": "https://repo.huaweicloud.com/repository/pypi/simple/",
  "/ali": "https://mirrors.aliyun.com/pypi/simple/",
  "/alibaba": "https://mirrors.aliyun.com/pypi/simple/",
  "/ustc": "https://pypi.mirrors.ustc.edu.cn/simple/",
  "/tx": "https://mirrors.cloud.tencent.com/pypi/simple/",
}
```

## 国内常见的PyPI镜像加速

- 清华
  > `pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package`

- 中国科技大学
  > `pip install -i https://mirrors.ustc.edu.cn/pypi/web/simple some-package`

- 阿里云
  > `pip install -i https://mirrors.aliyun.com/pypi/simple some-package`

- 腾讯云
  > `pip install -i https://mirrors.cloud.tencent.com/pypi/simple some-package`
