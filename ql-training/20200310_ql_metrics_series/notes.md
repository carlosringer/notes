# QL Metrics Training Series

## Metrics, Logging, and Tracking

- Metrics (Aggregatable)
  - QL Metrics
- Logging (Events)
  - Splunk 
  - AWS X-Ray

## Introduction to InfluxDB

- open source time series database
- host level statistics from windows and linux
  - cpu
  - memory
  - disk
  - network
  - uptime
  - windows service statistics
- default to open
- can receive metrics from anywhere (AWS, on prom, etc)
- time Series
  - a run or series of data points indexed in time order
- data Point
  - discrete unit of information, for analytics (measurement)
- data is stored by
  - Fields and Tags
  - Tags
    - store and indexed in memory
    - fast and easy retrieval
  - Tag Set
    - tag key (metadata name)
    - tag values (metadata)
- metadata is a set of data that provides information about other data
- required tags
  - operation
  - category
  - type
  - host
  - result
  - app-id
  - location
  - environment
- tags are a way to help filter
- tag set information is stored in influxDB as a measurement
- measurements have a retention policy
  - tells InfluxDB how long to keep data ands how many copies
  - current retention policy is 5 weeks
- InfluxDB data is organized as a Schema
- points represent a single data record
- points include four components
  - measurement
  - tag set
  - field set
  - timestamp
- points are uniquely identified by its series and timestamp
- represented by one row in "line protocol"
  - text-based format for writing points

## Intro to Grafana

- open source metrics tool
- shorty/grafana
- ql metrics platform is default to open
- best practices
  - create a folder by team name
  - tag the dashboard using relevant terms
    - environment
    - application core id
- agent only updates every 10s
  - queries below that time will not yield data
