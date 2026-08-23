# INCE - AI创作平台

基于 VOZEB PRO 的企业级AI创作平台

## 仓库信息

- **主仓库**: https://github.com/1240052492/INCE
- **生产分支**: `main-product` (受保护)
- **开发分支**: `main`

## 分支说明

### main-product（生产分支）
- ✅ 已启用分支保护
- ✅ 禁止强制推送
- ✅ 禁止删除
- ✅ 需要Pull Request审核后才能合并
- ⚠️ **仅用于生产环境部署，不允许直接提交**

### main（开发分支）
- 日常开发使用
- 测试通过后通过PR合并到 main-product

## 部署架构

- **服务器**: txy1 (43.162.93.138)
- **Web端口**: 443 (HTTPS)
- **数据库**: PostgreSQL
- **反向代理**: Nginx
- **容器化**: Docker + Docker Compose

## 安全配置

- ✅ HTTPS已启用（自签名证书）
- ✅ HTTP自动重定向到HTTPS
- ✅ 数据库密码加密存储
- ✅ 管理员权限细粒度控制

## 管理后台

- **访问地址**: https://43.162.93.138/admin
- **管理员账号**: sss
- **权限**: system, users, billing, generation, announcements, settings

## 存储配置

- **当前方式**: 本地文件系统存储
- **路径**: `/app/web/.data/`
- **支持扩展**: COS/OSS/S3对象存储

## 版本信息

- **VOZEB PRO版本**: v0.0.6
- **部署时间**: 2026-08-23
- **最后更新**: 2026-08-23

---

**注意**: 所有生产环境变更必须通过Pull Request流程，经过审核后才能合并到 main-product 分支。
