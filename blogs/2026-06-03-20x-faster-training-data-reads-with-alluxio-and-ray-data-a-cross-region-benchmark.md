---
title: "20x Faster Training Data Reads with Alluxio and Ray Data: A Cross-Region Benchmark"
url: "https://www.anyscale.com/blog/20-times-faster-cross-region-training-data-reads-alluxio-ray-on-anyscale"
date: "2026-06-03"
author: "Elizabeth Hu, Nick Gupta, Bin Fan, and David Zhu"
feed_url: "https://www.anyscale.com/sitemap.xml"
---
This benchmark demonstrates how deploying Alluxio as a distributed NVMe cache alongside Ray clusters dramatically accelerates cross-region data access. When reading 1TB of Parquet files from Google Cloud Storage in a different region, warm cache reads achieved a 20x speedup, dropping from 4,241 seconds to 208 seconds. The article details technical pitfalls encountered during testing and recommends using .map_batches().count() instead of .materialize() for accurate benchmarking.
