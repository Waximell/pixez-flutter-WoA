# MSIX 证书

`pixez-woa.cer` 是本项目 MSIX 包的公钥证书（自签）。

- 发布者主体：`CN=Waximell, C=CN`
- 指纹：`B1C5C4F56505E5F910FCEB32BC77E2E20C7EDBEB`
- 有效期至：2036-11-17

自签证书需要手动信任后才能安装对应 MSIX：

```powershell
Import-Certificate -FilePath .\pixez-woa.cer -CertStoreLocation Cert:\CurrentUser\TrustedPeople
```

私钥（`.pfx`）不在仓库中，不要提交。
