# 数据库迁移

### 数据库升级迁移（仅升级系统版本时执行）

数据库升级脚本尽量会保持兼容，如果因其他因素导致不可兼容升级，会在升级文档中着重说明。

#### 确定升级的版本

首先确定要升级的系统版本，例如当前版本为 v1.0，要升级的目标版本为 v1.1，执行 src/backend/database/migrations/v1.0_v1.1 目录下的
sql 文件即可。其中ddl.sql 为表结构迁移相关文件, dml.sql 为数据文件。

