# CityMesh.AI 协议技术草案（v0.1）

## 1. 目标
让消费者AI与商户AI通过**统一语义**与**标准机制**完成自治交易。

## 2. 语义层（JSON-LD 最小集）
```json
{
  "@context": "https://schema.citymesh.ai/v1",
  "type": "NegotiationRequest",
  "serviceType": "yoga.class",
  "timeWindow": {"start":"2025-10-31T18:00:00-06:00","end":"2025-10-31T21:00:00-06:00"},
  "price": {"target":25,"ceiling":30,"currency":"CAD"},
  "options": {"urgency":"normal","addons":[]},
  "trust": {"score":0.72,"proofs":[]},
  "callback": "https://your-site.com/a2a/callback"
}
