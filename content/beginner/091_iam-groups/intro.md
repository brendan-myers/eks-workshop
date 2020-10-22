---
title: "Kubernetes Authentication"
date: 2020-04-05T18:00:00-00:00
draft: false
weight: 10
---

In the [intro to RBAC](/beginner/090_rbac/) module, we have seen how we can give individual users access to Kubernetes.

If you have multiple teams which each require different cluster access permissions, it would be difficult to manually add or remove access for every EKS cluster.

We can leverage AWS [IAM Groups](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_groups.html) to easily add or remove users and give them permission to whole cluster, or just part of it depending on which groups they belong to.

In this lesson, we will create 3 IAM roles that we will map to 3 IAM groups.
