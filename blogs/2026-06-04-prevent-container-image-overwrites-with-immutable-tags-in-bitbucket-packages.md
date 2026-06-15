---
title: "Prevent container image overwrites with immutable tags in Bitbucket Packages"
url: "https://www.atlassian.com/blog/bitbucket/prevent-container-image-overwrites-with-immutable-tags-in-bitbucket-packages"
date: "2026-06-04"
author: ""
feed_url: "https://atlassianblog.wpengine.com/feed/"
---
Bitbucket Packages now supports immutable tags for the container registry, allowing administrators to prevent accidental overwrites of container images through customizable protection rules for production and release deployments. Once an immutable tag is set, the tag cannot be overwritten after the initial push, improving reproducibility and compliance for CI/CD pipelines. Admins can configure protection rules at the repository level to enforce immutability for specific tag patterns like production or release builds.
