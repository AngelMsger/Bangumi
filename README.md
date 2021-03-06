# Bangumi-Provider
[![Build Status](https://travis-ci.org/AngelMsger/Bangumi-Provider.svg?branch=master)](https://travis-ci.org/AngelMsger/Bangumi-Provider)

![Bangumi-Crawler](https://s1.hdslb.com/bfs/static/jinkela/home/images/bgm-nodata.png)

## Overview
Bangumi-Provider is a content provider for [Bangumi-Visualizer](https://github.com/AngelMsger/Bangumi-Visualizer). It crawl, analyze the data from [Bilibili](https://www.bilibili.com), and persist the result to database, using [Collaborative Filtering](https://www.wikiwand.com/en/Collaborative_filtering) algorithm when analyzing data. It run with single thread and no framework was used.

## Features
* Incremental Crawl & Analyze
* Multi Storage Backend Support
* Containerized

## Usage

### With Docker-Compose
`docker-compose up`

### With Docker
`docker run -itd --name=provider --net=host -e DB_PASSWORD=$DB_PASSWORD angelmsger/bangumi-provider`

### Manually
`python -m venv venv && source venv/bin/activate && pip install -r requirements && python exec.py`

## Todo
1. MySQL support
2. Concurrent feature

## Quote
1. Use [Kaaass](kaaass.net)'s API when auth after v1.3.x.
