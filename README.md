# walfree-2.3TB — 公开工业测试数据集（匿名发布）
# Public Industrial Test Dataset — SQLite WAL Stress Corpus (2.31 TB)

## 这是什么 / What this is
7 组 SQLite 数据库三件套（`.db` + `.db-shm` + `.db-wal`），其中 WAL（预写日志）单体最大 481 GB。
21 个文件，合计 **2,312,156,895,720 字节（2.31 TB / 2.10 TiB）**，逐字节核验。
A set of 7 SQLite database triplets (db + shm + wal) with extremely large write-ahead logs (up to 481 GB each), 21 files, 2.31 TB total, byte-verified.

## 用途 / Use cases
- 带宽 / 磁盘吞吐基准测试（throughput benchmark）
- CDN、对象存储、P2P 分发压测（distribution stress test）
- SQLite WAL 恢复 / checkpoint / 崩溃一致性研究（WAL recovery stress）
- 下载器分块、断点续传、校验工具链测试（chunking / resume / verify tooling）

## 获取方式 A：HTTPS 直链（免鉴权，支持 Range，HEAD/GET 均可）/ Direct HTTPS links
托管于华为云 OBS（cn-north-4），公共读，无签名不过期。

| 文件 | 字节数 | 约 |
|---|---:|---:|
| `walfree.db` | 16,384 | 0.00 GB |
| `walfree.db-shm` | 1,002,700,800 | 1.00 GB |
| `walfree.db-wal` | 516,375,280,752 | 516.38 GB |
| `shard0.db` | 16,384 | 0.00 GB |
| `shard0.db-shm` | 571,441,152 | 0.57 GB |
| `shard0.db-wal` | 294,276,145,912 | 294.28 GB |
| `shard1.db` | 16,384 | 0.00 GB |
| `shard1.db-shm` | 539,590,656 | 0.54 GB |
| `shard1.db-wal` | 277,887,082,552 | 277.89 GB |
| `shard2.db` | 16,384 | 0.00 GB |
| `shard2.db-shm` | 546,996,224 | 0.55 GB |
| `shard2.db-wal` | 281,690,938,472 | 281.69 GB |
| `shard3.db` | 16,384 | 0.00 GB |
| `shard3.db-shm` | 619,282,432 | 0.62 GB |
| `shard3.db-wal` | 318,915,566,952 | 318.92 GB |
| `shard4.db` | 16,384 | 0.00 GB |
| `shard4.db-shm` | 610,533,376 | 0.61 GB |
| `shard4.db-wal` | 314,419,493,352 | 314.42 GB |
| `shard5.db` | 16,384 | 0.00 GB |
| `shard5.db-shm` | 590,512,128 | 0.59 GB |
| `shard5.db-wal` | 304,111,216,272 | 304.11 GB |

直链列表 / Plain URLs:
```
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/walfree.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/walfree.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/walfree.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard0.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard0.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard0.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard1.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard1.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard1.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard2.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard2.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard2.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard3.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard3.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard3.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard4.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard4.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard4.db-wal
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard5.db
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard5.db-shm
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/shard5.db-wal
```

## 获取方式 B：BitTorrent
.torrent 文件直链 / Torrent file:
https://k3-walfree-rescue-n4-2026-09-13.obs.cn-north-4.myhuaweicloud.com/walfree_xunlei_v2_2026-09-13.torrent

info-hash: `c72f58acffe1acb990965549ee6d56c9864792bd`（23 trackers）

magnet:
```
magnet:?xt=urn:btih:c72f58acffe1acb990965549ee6d56c9864792bd&dn=walfree%E5%AE%9E%E9%AA%8C%5F2026-09-12&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce&tr=udp%3A%2F%2Fopen.tracker.cl%3A1337%2Fannounce&tr=udp%3A%2F%2Fexplodie.org%3A6969%2Fannounce&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A6969%2Fannounce&tr=udp%3A%2F%2Fzer0day.ch%3A1337%2Fannounce&tr=udp%3A%2F%2Ftracker.therarbg.to%3A6969%2Fannounce&tr=udp%3A%2F%2Ftracker.publictracker.xyz%3A6969%2Fannounce&tr=udp%3A%2F%2Fopen.demonii.com%3A1337%2Fannounce&tr=udp%3A%2F%2Fopen.stealth.si%3A80%2Fannounce&tr=udp%3A%2F%2Ftracker.torrent.eu.org%3A451%2Fannounce&tr=udp%3A%2F%2Ftracker.qu.ax%3A6969%2Fannounce&tr=udp%3A%2F%2Ftracker.corpscorp.online%3A80%2Fannounce&tr=udp%3A%2F%2Ftracker.auctor.tv%3A6969%2Fannounce&tr=udp%3A%2F%2Ftracker-udp.gbitt.info%3A80%2Fannounce&tr=udp%3A%2F%2Fleet-tracker.moe%3A1337%2Fannounce&tr=udp%3A%2F%2Fexodus.desync.com%3A6969%2Fannounce&tr=udp%3A%2F%2Fbittorrent-tracker.e-n-c-r-y-p-t.net%3A1337%2Fannounce&tr=https%3A%2F%2Ftracker.zhuqiy.com%3A443%2Fannounce&tr=https%3A%2F%2Ftracker.pmman.tech%3A443%2Fannounce&tr=https%3A%2F%2Ftracker.nekomi.cn%3A443%2Fannounce&tr=https%3A%2F%2Ftracker.bt4g.com%3A443%2Fannounce&tr=https%3A%2F%2Fht.therarbg.to%3A443%2Fannounce&tr=https%3A%2F%2F004430.xyz%3A443%2Fannounce
```

## 完整性 / Integrity
上表字节数即首要校验；sha256 清单稍后补挂（sizes are the primary check; sha256 manifest to be appended）。

## 条款 / Terms
公开测试数据，任意用途免费使用，无任何担保。欢迎镜像与做种。
Public test data. Free for any use, no warranty. Mirrors and seeders welcome.
出口流量由发布方按量付费——若您拉大件，请顺手给 BT 做种，让更多人从 P2P 而非源站取数。
Egress is metered; if you pull the big files, please seed the torrent.
