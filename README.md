## 利用RPC添加计划任务


事件的起因是有某学员通过飞书的权限控制不严格，偷取我个人笔记的里面记录，拿去某vx群倒卖，倒卖价格让人乍舌，500RMB/650RMB 就卖，所以决定公开这种方法

方法存在时效性，肯定会被安全厂商添加规则进行拦截，后续不会再发布任何关于核晶维权的绕过手法

要吃瓜的各位，请移步：http://archive.today/2026.05.16-155204/https://mp.weixin.qq.com/s/zOMxAEtOLXT3zwUf_jx2gw

利用RPC接口添加计划任务，源项目被360核晶拦截，将localhost修改为0或者NULL，即可绕过核晶拦截
```
RpcStringBindingComposeW(RPC_UUID, (RPC_WSTR)L"ncacn_np", (RPC_WSTR)NULL, InterfaceAddress, NULL, &StringBinding);
```
