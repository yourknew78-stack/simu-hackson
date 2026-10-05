# main.md · 主分支接力日志

> 本文件位于 `main` 分支，是接力赛的起点与主交接看板。

## 一、接力棒信息

| 项目 | 值 |
| --- | --- |
| 赛事 | GitLab 模拟接力 |
| 起始分支 | `main` |
| 当前持有人 | 林一棒（alice） |
| 交接状态 | 待交接 |

## 二、接力规则

1. 每人在自己的特性分支上提交，**不直接推 `main`**。
2. 完成后发 Merge Request，由下一位选手 Review。
3. Review 通过后合并回 `main`，接力棒交给下一位。

## 三、交接记录

| 棒次 | 选手 | 分支 | 产出 |
| --- | --- | --- | --- |
| 1 | 林一棒 (alice) | `main` | `main.md` |
| 2 | 陈二棒 (bob) | `branch1` | `branch1.md` |
| 3 | 王三棒 (carol) | `branch1` | `branch1.md` 接力区段落 |

## 四、怎么跑起来

```bash
# 完整演练一遍接力流程（会在 ./relay-demo 里建一个独立仓库）
./simulate-relay.sh

# 换目录 / 换人数
./simulate-relay.sh --workdir /tmp/relay --runners 4

# 演练完直接推到远端
./simulate-relay.sh --push git@github.com:USERNAME/relay-demo.git
```

详见 [README.md](README.md)。
