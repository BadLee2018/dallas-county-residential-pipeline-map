# Dallas County 住宅开发管线地图

本仓库只发布去标识化、subdivision-level 聚合的 WGS84 GeoJSON，用于 Dallas County GIS 数据挑战。文件不包含 owner、taxpayer 或 mailing-address 字段。

浏览器展示 geometry 使用 10-foot topology-preserving simplification。项目统计与业务属性不变；presentation 文件只增加显示样式与排名 marker。

## 地图

- [presentation_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_active_residential_presentation.geojson) - 401 个 Active Residential 项目，Top 5 高亮。
- [top5_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_top5_residential_projects.geojson) - Top 5 边界与排名 marker。
- [full_audit_map](https://geojson.io/#data=data:text/x-url,https%3A%2F%2Fraw.githubusercontent.com%2FBadLee2018%2Fdallas-county-residential-pipeline-map%2Fmain%2Fdallas_residential_pipeline_display.geojson) - 全部 1,477 个高置信项目。

## 口径与限制

- 结果是严格空间门禁后的高置信子集，不代表 Dallas County 全量覆盖。
- `active_residential` 由 recent official structure evidence 支持，是 activity proxy，不等同于 building permit 结论。
- Source 中缺失的 subdivision number 和 city 保持 null，不进行推断。
- Multi-Family parcel 不转换为一个 household；缺少官方 `NUM_UNITS` 时保持 null。
