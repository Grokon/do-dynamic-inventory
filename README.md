# do-dynamic-inventory
Ansible AWX DigitalOcean dynamic inventory


!!!test repo




## AWX: Custom credential:

### Input configuration:

```yaml
fields:
  - id: api_token
    type: string
    label: DO_API_TOKEN
    secret: true
required:
  - api_token
```

### Injector configuration:

```yaml
env:
  DO_API_TOKEN: '{{ api_token }}'
```
