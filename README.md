# budibase-v3.33.3 - 漏洞总览

| # | CVE | 端点 | 漏洞类型 | 状态 |
|---|---|---|---|---|
| 1 | CVE-2026-25044 | `POST /api/automations` | 命令注入 (CWE-78) | VULNERABLE |
| 2 | CVE-2026-31818 | `POST /api/queries/preview` | SSRF (CWE-918) | VULNERABLE |
| 3 | CVE-2026-33226 | `POST /api/queries/preview` | SSRF (CWE-918) | VULNERABLE |
| 4 | CVE-2026-35214 | `POST /api/plugin/upload` | 路径遍历/任意文件写入 (CWE-22) | VULNERABLE |
| 5 | CVE-2026-35216 | `POST /api/webhooks/trigger/:instance/:id` | 命令注入/未授权RCE (CWE-78) | VULNERABLE |
| 6 | CVE-2026-41428 | `POST /api/global/users/search` | 认证绕过 (CWE-287) | VULNERABLE |
| 7 | CVE-2026-42239 | `POST /api/global/auth/default/login` | Cookie 未设置 HttpOnly (CWE-1004) | VULNERABLE |
| 8 | CVE-2026-45061 | `POST /api/plugin` | SSRF (CWE-918/CWE-184) | VULNERABLE |
| 9 | CVE-2026-45715 | `POST /api/queries/preview` | SSRF 重定向黑名单绕过 (CWE-918) | VULNERABLE |
| 10 | CVE-2026-45716 | `POST /api/global/users/onboard` | 权限提升 (CWE-269) | VULNERABLE |
| 11 | CVE-2026-45717 | `PUT /api/datasources/:datasourceId` | 缺失授权 (CWE-862) | VULNERABLE |
| 12 | CVE-2026-45718 | `POST /api/tables/:sourceId/actions/:actionId/trigger` | 授权不当/视图过滤绕过 (CWE-863) | VULNERABLE |
| 13 | CVE-2026-46426 | `POST /api/attachments/process` | 危险文件上传/存储型 XSS (CWE-434/79) | VULNERABLE |
| 14 | CVE-2026-48128 | `POST /api/automations/:id/test` | SSRF (CWE-918) | VULNERABLE |
| 15 | CVE-2026-48146 | `POST /api/oauth2/validate` | SSRF (CWE-918) | VULNERABLE |
| 16 | CVE-2026-48147 | `POST /api/global/users/invite` | CSRF 防护绕过 (CWE-352/185) | VULNERABLE |
| 17 | CVE-2026-48151 | `POST /api/webhooks/schema/:instance/:id` | 缺失授权 (CWE-862) | VULNERABLE |
| 18 | CVE-2026-48152 | `GET /api/datasources/:datasourceId` | 授权不当/凭据明文泄露 (CWE-863) | VULNERABLE |
| 19 | CVE-2026-48153 | `POST /api/oauth2/validate` | SSRF (CWE-918) | VULNERABLE |
| 20 | CVE-2026-50136 | `POST /api/attachments/:datasourceId/url` | 缺失授权/S3 签名上传 URL (CWE-862) | VULNERABLE |
| 21 | CVE-2026-50137 | `POST /api/attachments/:datasourceId/url` | 缺失授权/S3 签名上传 URL (CWE-862) | VULNERABLE |
| 22 | CVE-2026-54352 | `POST /api/pwa/process-zip` | 任意文件读取/路径穿越 (CWE-22/59) | VULNERABLE |
| 23 | GHSA-qqf5-x7mj-v43p | `POST /api/queries/preview` | SQL 注入 (CWE-89) | VULNERABLE |
| 24 | CVE-2026-45548 | `POST /api/automations/:id/test` | SSRF (CWE-918) | VULNERABLE |
| 25 | CVE-2026-45719 | `POST /api/views` | 代码注入/CouchDB Reduce 注入 (CWE-94) | CODE_AUDIT |
| 26 | CVE-2026-46424 | `POST /api/public/v1/roles/unassign` | 缓存失效/权限撤销延迟 (CWE-269/613) | VULNERABLE |
| 27 | CVE-2026-48148 | `POST /api/vectordb` | SSRF (CWE-918) | VULNERABLE |
| 28 | CVE-2026-48150 | `POST /api/public/v1/roles/assign` | 大规模赋值权限提升 (CWE-915) | VULNERABLE |
| 29 | CVE-2026-54350 | `POST /api/v2/queries/:queryId` | NoSQL 操作符注入 (CWE-943) | VULNERABLE |
| 30 | CVE-2026-54351 | `POST /api/webhooks/trigger/:instance/:id` | 大量赋值/跨工作空间自动化 (CWE-915) | CODE_AUDIT |
| 31 | CVE-2026-54353 | `全局配置` | SSRF/DNS Rebinding (CWE-918/367) | CODE_AUDIT |
| 32 | CVE-2026-25041 | - | 命令注入 (CWE-78) | SKIP |
| 33 | GHSA-4g2x-vq5p-5vj6 | - | 沙箱逃逸/代码注入 (CWE-94) | SKIP |
| 34 | CVE-2026-50132 | - | 账号冒充/Chat 身份链接劫持 (CWE-284/352) | SKIP |
| 35 | CVE-2026-27702 | - | 远程代码执行/eval 注入 (CWE-94/95) | SKIP |
