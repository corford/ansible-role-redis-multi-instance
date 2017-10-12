# Ansible Role: redis-multi-instance

Ansible role to compile and install redis (designed to be called as a dependency
of a "redis-child-instance" role).

This role will create a systemd target group for any future redis instance(s) to
join. All child members can then be controlled with a single command:

```
systemctl [start|stop|restart] redis.target
```

Note: This role intentionally does not setup or configure a redis instance

## License

MIT / BSD
