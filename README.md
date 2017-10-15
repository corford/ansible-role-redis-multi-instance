# Ansible Role: redis-multi-instance

Ansible role to compile and install redis (for later use by "redis-instance" roles).

This role also creates a systemd target group for any future redis instance(s) to
join. All members can then be controlled with a single command:

```
systemctl [start|stop|restart] redis.target
```

Note: This role intentionally does not setup or configure any redis instances.

## License

MIT / BSD
