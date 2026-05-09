---
title: "ActiveObjects streaming API"
url: "http://blogs.atlassian.com/developer/2011/09/activeobjects_streaming_api.html"
date: "2011-09-30"
author: "Alex Hennecke"
feed_url: "https://blog.developer.atlassian.com/atom.xml"
---
We recently overhauled the GreenHopper ranking implementation, and the new "Global Rank" that's used on the Rapid Board is relying on ActiveObjects (AO) as data storage. Since we're storing and reading large amounts of data (at least one row per issue), we've been hitting the limits of AO's read capabilities. Reading from ActiveObjects When using AO, you define an interface of your entity with some annotations that influence how it's mapped to the database table AO manages. This is the interface for GreenHopper's Global Rank entity: With adding this to atlassian-plugins.
