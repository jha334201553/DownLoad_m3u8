2018.9.29
1. 完成 m3u8 下载代码

2018.9.30
1. 完成多线程下载，并列表保存以后依次保存到文件中

2018.10.8
1. 修复知乎上带有auth_key参数的ts下载失败问题
2. 修复m3u8文件地址以斜杆/开头的需要解析成host的绝对地址，而不是相对当前URL的地址

2019.3.29
1. 更新m3u8文件带有AES-128加密的ts文件下载并解密工作 

2019.6.5
1. 每个ts数据块都添加一个解密标记，如果在EXT-X-KEY之前的ts块是没有加密的，所以不需要解密
2. 设定一个aes解码失败的计数器nDecodeErrCount，超过三次解码失败，跳过解码

2019.7.11
1. 添加可以略过某几个帧的命令行参数，为了不下载开头部分带广告的帧

2019.10.11
1. 有多个.的情况下取第一个点后面的作为后缀搜索 

2019.12.21
1. 修补URL中带有端口号时解析错误
