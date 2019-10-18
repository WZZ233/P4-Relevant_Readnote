# Stateless Datacenter Load-balancing with Beamer

## Abstract & Introduction

**Target**: Load balancing in Datacenters.

**Existing solutions**: They all keep per-flow state: after a load balancer decides which server should handle a connection, that decision is “remembered” locally and used to handle future packets of the same connection.

**Pros of stateful**: Ensure that ongoing connections do not break when servers and muxes come or go.

**Cons of stateful**:
1. Standard scaling events break many ongoing connections.
2. SYN flood attacks prevent muxes from keeping “good” connection state, negating its benefits.
----
*My question: What is SYN flood attacks?*
----
3. Running stateful load-balancers in software with many flows reduces throughput.
----
*My question: Why must software?*



