



```markdown

&nbsp;

Ecommerce Data Warehouse \& Analytics (电商用户行为数仓)



项目介绍

基于模拟的千万级电商用户行为日志（User Behavior Log），本项目模拟了企业级数据仓库的搭建流程。实现了从 ETL 数据清洗、数仓分层建模 (ODS/DWD/DWS) 到 商业指标计算 的全链路数据处理。



核心工作

1\.  ETL Pipeline: 使用 Python (Pandas) 清洗原始 CSV 数据，处理缺失值与异常时间戳，完成数据规范化。

2\.  数仓分层架构: 设计了 ODS -> DWD -> DWS -> ADS 四层架构，模拟 Hive 数仓流转。

3\.  维度建模: 基于 Kimball 星型模型 理论，构建了订单事实表与维度表。

4\.  指标分析:使用 SQL 实现 漏斗模型 (Funnel)、留存率 及 RFM 用户价值分析。



技术栈

Language: Python 3.9, SQL

Libraries: Pandas, NumPy, SQLAlchemy, Matplotlib/Seaborn

Database: SQLite (模拟 Hive/MySQL)

Architecture: Star Schema, Data Warehouse Layering



数仓架构 (Schema)

ODS: `ods\_raw\_log` (原始日志)

DWD: `dwd\_fact\_order` (事实表), `dim\_user`, `dim\_product` (维度表)

DWS: `dws\_daily\_traffic` (每日流量汇总)

ADS: `ads\_conversion\_rate` (转化率报表)





