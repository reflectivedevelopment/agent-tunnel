# agent-tunnel

This is to form a connection to a localtunnel, and allow the client application to discover the url that you are connecting to.

Using docker-compose, you can run it like the following, and then use a client script to fetch the url.

```
  tunnel-test:
    image: reflectivedevelopment/agent-tunnel
    command: "agent-test:3007 -p 4040 --host ${AGENT_TUNNEL_HOST}"
```
