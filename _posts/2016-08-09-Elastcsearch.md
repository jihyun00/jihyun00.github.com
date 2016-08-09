---
layout: page
title: PROJECT
permalink: /project
---

# ElasticSearch

회사에서 Kafka에 있는 데이터를 Elasticsearch로 옮기는 API를 개발하였다.

Bulk API를 사용하면서 간략한 이슈가 있었는데,

Bulk API를 이용할 때 데이터가 반드시,

```
{ "index" : { "_index" : "test", "_type" : "type1", "_id" : "1" } }
{ "field1" : "value1" }
{ "index" : { "_index" : "test", "_type" : "type1", "_id" : "2" } }
{ "field1" : "value1" }

```
이와 같은 형태로 들어가야 한다는 것.

즉, 각각의 데이터에 대해 _index, _type, _id 데이터가 포함되어야 함. 

