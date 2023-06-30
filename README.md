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


## 国内常见的PyPI镜像加速

- 清华
  > `pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package`

- 中国科技大学
  > `pip install -i https://mirrors.ustc.edu.cn/pypi/web/simple some-package`

- 阿里云
  > `pip install -i https://mirrors.aliyun.com/pypi/simple some-package`

- 腾讯云
  > `pip install -i https://mirrors.cloud.tencent.com/pypi/simple some-package`
