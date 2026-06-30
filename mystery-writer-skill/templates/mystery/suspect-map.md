# 嫌疑人谱系与矛盾网络

> 专门用于梳理“所有人都有动机，所有人都有秘密”的社会关系网络。

```json
// 供 AI 高效读取的图结构 JSON 数据区
{
  "nodes": [
    {"id": "CH_001", "name": "侦探", "type": "detective"},
    {"id": "CH_002", "name": "死者", "type": "victim"},
    {"id": "CH_003", "name": "嫌疑人A", "type": "suspect", "alibi": "verified"}
  ],
  "edges": [
    {"source": "CH_003", "target": "CH_002", "relation": "债权人", "tension": "high"}
  ]
}
矛盾冲突点清单

    [嫌疑人 A -> 死者]：经济纠纷。死者掌握了 A 挪用公款的证据。

    [嫌疑人 B -> 嫌疑人 C]：情人关系。案发当晚互相作伪证。