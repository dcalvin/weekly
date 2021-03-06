---
title: Weekly update (July 23 ~ July 29, 2018)
date: 2018-07-30
summary: Last week, we landed 43 PRs in the TiDB repositories, 6 PRs in the TiSpark repositories, and 17 PRs in the TiKV and PD repositories.
tags: ['TiDB', 'TiKV', 'PD', 'TiSpark']
---

# Weekly update in TiDB

Last week, we landed [43 PRs](https://github.com/pingcap/tidb/pulls?utf8=%E2%9C%93&q=is%3Apr+is%3Amerged+merged%3A2018-07-23..2018-07-29+) in the TiDB repositories.

## Added

- [Add the `sum_decimal` method for `AggFunc`](https://github.com/pingcap/tidb/pull/7096)
- [Support truncating and dropping partitioned tables](https://github.com/pingcap/tidb/pull/7036)
- [Implement the reorganization of table partition when adding the index](https://github.com/pingcap/tidb/pull/6814)

## Fixed

- [Fix a bug that the `bit` and `year column` types are not supported when a partition table is created](https://github.com/pingcap/tidb/pull/7122)
- [Fix a bug in the decimal modulo operation](https://github.com/pingcap/tidb/pull/7113)
- [Refactor the code of building `Insert`](https://github.com/pingcap/tidb/pull/7068)
- [Fix a panic caused by the outdated feedback](https://github.com/pingcap/tidb/pull/7128)
- [Fix a panic that is upgraded from the old version TiDB](https://github.com/pingcap/tidb/pull/7136)
- [Fix a bug that null values cannot be found using the unique index](https://github.com/pingcap/tidb/pull/7163)

## Improved

- [Add the partition function check when creating a partition table](https://github.com/pingcap/tidb/pull/7111)
- [Provide preliminary support for the parallel DDL operation](https://github.com/pingcap/tidb/pull/6955)
- [Use `feedback` timely](https://github.com/pingcap/tidb/pull/6859)
- [Optimize `DecodeRowKey`](https://github.com/pingcap/tidb/pull/7149)
- [Remove the `types.Row` interface](https://github.com/pingcap/tidb/pull/7170)
- [Pass `row pointer` rather than `row` to avoid `convertT2I`](https://github.com/pingcap/tidb/pull/7143)

# Weekly update in TiSpark

Last week, we landed [6 PRs](https://github.com/pingcap/tispark/pulls?utf8=%E2%9C%93&q=is%3Apr+is%3Amerged+merged%3A2018-07-23..2018-07-29) in the TiSpark repositories.

## Fixed

- [Fix a decimal decoding bug](https://github.com/pingcap/tispark/pull/401)

# Weekly update in TiKV and PD

Last week, we landed [17 PRs](https://github.com/search?utf8=%E2%9C%93&q=repo%3Apingcap%2Ftikv+repo%3Apingcap%2Fpd+is%3Apr+is%3Amerged+merged%3A2018-07-23..2018-07-29) in the TiKV and PD repositories.

## Added

- [Support encoding and decoding a Chunk](https://github.com/pingcap/tikv/pull/3332)
- [Introduce a version check mechanism](https://github.com/pingcap/pd/pull/1148)
- [Add thread I/O metrics](https://github.com/pingcap/tikv/pull/3338)
- [Add a document about the PD API](https://github.com/pingcap/pd/pull/1105)

## Fixed

- [Fix a bug in `AdjacentRegionScheduler`](https://github.com/pingcap/pd/pull/1158)

## Improved

- [Keep the number of operators generated by `HotRegionScheduler` within the schedule limit](https://github.com/pingcap/pd/pull/1155)
- [Stop searching in `get_txn_commit_info`](https://github.com/pingcap/tikv/pull/3308)
- [Check the legality of the label](https://github.com/pingcap/pd/pull/1154)
- [Escape key in `Error`](https://github.com/pingcap/tikv/pull/3361)
- [Refine the task log in `raftstore`](https://github.com/pingcap/tikv/pull/3339)

# New contributor (Thanks!)

- tidb: [laidahe](https://github.com/laidahe)
