# LGD — Lifecycle Governance Doctrine（生命周期全程治理理论）

> You don't have to believe in it. Try to break it.
> 你不必先认同它，先试着打破它。

LGD 是一套关于「自治之物（agent / 智能体 / 自治系统）在其整个生命周期内如何被治理」的理论框架。
本仓是它的**公开入口与贡献体系**：任何人都可以运行、攻击、或扩展它。

---

## Run it in 3 minutes

```bash
# 1. 取得国际自治之物挑战赛（UIBC）协议与参考实现
git clone https://github.com/zhaoxinghua09-cell/uibc-core
cd uibc-core
# 2. 运行一致性自检
python -m unittest discover tests
# 3. 运行独立校验器
python independent_verifier/cross_check.py
```

可复算指针：仓库 `uibc-core`（Apache-2.0）；概念 DOI `10.5281/zenodo.22821834`；Sigstore Rekor `logIndex 2883389783`。

---

## Three doors（三个入口）

| 入口 | 面向 | 你拿到的 | 判定 |
|---|---|---|---|
| **RUN IT** | 任何能开终端的人 | 克隆 → 一条命令跑起来 → 可运行证据（输出 / 退出码 / 版本号） | 最低门槛：证明"不是纸上的" |
| **BREAK IT** | 红队 / 逆向 / 怀疑派 | **不需要先认同理论**，直接攻击、找 silent failure → 失败案例（可复现步骤 + 期望 vs 实测） | 提供对理论的证伪路径 ⇒ 最高价值 |
| **BUILD IT** | 工程师 | 写代码 / adapter / 案例 → PR | 生态形成的信号 |

---

## The tree（结构）

> 体例（《命名体例规范》v1.0 R-STYLE-1）：下列为**概念名/层名**，非仓库名；仓名一律以 `owner/repo` 全形另列。

```
Theory    → LGD（规范文本，保留所有权利）
Protocol   → UIBC（国际自治之物挑战赛 / 一致性与越权用例）
Verification → Silent Failure Catalog · Assayance
Agent Layer → Skills · Memory
Benchmark  → UIBC-Benchmark-Spec（**规格件名，非 repository**；内部工作稿，非对外发布物）
Applications → MedXpert（生产参考部署，自报）
```

---

## Contribute（贡献）

- 流程见 [CONTRIBUTING.md](CONTRIBUTING.md)
- 贡献者阶梯见 [CONTRIBUTOR-LADDER.md](CONTRIBUTOR-LADDER.md)（L1 Explorer → L5 Independent Verifier）
- 贡献者契约（CLA）见 [CONTRIBUTOR-AGREEMENT.md](CONTRIBUTOR-AGREEMENT.md)
- 安全问题见 [SECURITY.md](SECURITY.md) · 行为准则见 [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

> 说明：我们**不承诺任何称号**。贡献者名录基于真实、可核验的贡献记录；名录条目可撤、可重算。
> 独立验证与公开致谢**仅在有真实第三方行为时发生**——我们不预先制造任何证据。

---

<!-- ===== 权属块（照抄 LGD对外表述规范_v1.3 §3.2，禁自拟） ===== -->
© 2026 赵兴华 / Steven Zhao·China (ORCID 0009-0001-0512-1237). All rights reserved.
理论署名 (attribution) : LGD（Lifecycle Governance Doctrine / 全程治理论）— SynomosAI initiative
名称状态 (name status)  : "SynomosAI" / "MedXpert" — 未申请实体注册、未申请商标注册
                        (not a registered legal entity; no trademark registered)
生产参考部署 (production reference, self-reported) : MedXpert
                    ← 非认证、非背书、非监管认可（not a certification or endorsement）

代码许可 (code license) : 本仓代码与文档示例 Apache-2.0（see LICENSE）
                    本仓所含 LGD 理论表述文本不在 Apache-2.0 覆盖范围内，保留所有权利
引用格式 (cite as)      : 本仓无独立 DOI —— 请引用理论真源 zhaoxinghua09-cell/lgd-theory · concept DOI 10.5281/zenodo.22456647
首次公开锚 (first public): 2026-10-02 · commit b40b38b · github.com/zhaoxinghua09-cell/LGD（public）
                    外锚 (external anchor): 无
