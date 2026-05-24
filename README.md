# AIWear Performance Test Attachments

本仓库用于保存 AIWear 项目接口性能测试的附件材料。

报告正文位于在线文档中，本仓库仅保存可复查和复现实验的测试附件，包括：

- `性能测试/jmx/`：JMeter 测试脚本。
- `性能测试/data/`：CSV 测试数据示例。
- `性能测试/results/`：JTL 原始测试结果。
- `性能测试/reports/`：JMeter HTML 报告。

## 目录说明

```text
性能测试/
├─ jmx/
├─ data/
├─ results/
└─ reports/
   ├─ light_api/
   ├─ upload_search/
   ├─ mixed_scene/
   ├─ mixed_scene_5thread/
   ├─ ai_heavy/
   │  └─ ai_heavy_3_180s/
   ├─ full_flow_image_search/
   │  ├─ image-search-flow-2thread_15min/
   │  └─ image-search-flow-3thread-15min/
   └─ full-flow_text_search/
      └─ edit-2thread-15min/
```

## 说明

- `AIWear_轻量接口数据预置.jmx` 仅用于准备轻量接口测试数据，不是正式压测场景。
- CSV 文件已脱敏，密码、图片路径和 OSS URL 使用示例值替代。
- JMX 文件已将服务器地址替换为 `your-server-host`，复现测试时需要改成实际测试环境地址。
- JTL 文件已将 URL 中的服务器地址替换为 `your-server-host`，响应时间、错误率、吞吐等原始指标保持不变。
- HTML 报告用于查看 JMeter 生成的 Statistics、Response Times、Throughput 等结果页面。

