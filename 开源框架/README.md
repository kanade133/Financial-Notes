# 开源框架

- QuantConnect/Lean : 完整引擎框架，不可拆分使用，官方主推云端部署，通过config配置模块和环境(回测/实盘)，数据源使用DataFeed, DataQueue模块，策略使用Algorithm模块，带有多个模板策略，结果使用ResultHandler控制输出
- StockSharp : 有单独功能模块引用库，可图形化低代码开发策略，核心数据通信方式是Message基类，通过自定义Connector的Adapter修改数据源，自带WPF控件，通过自定义继承Strategy实现策略
- VN.py : 可独立运行或引用库，模块化程度也高，国产本地化程度高，自带CTP数据源，Python语言，通过自定义继承策略模板实现策略

# CTP

CTP-Api官方只有cpp版本，尝试寻找C#封装版本但都不太理想，没有简单易用或可用的，自己用也许得考虑使用swig等手段自己封装，py版本可以考虑直接用VN.py