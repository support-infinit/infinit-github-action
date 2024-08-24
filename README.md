# infinit GitHub Action

- run infinit image in a step.
- See https://github.com/support-infinit/infinit-github-action/blob/main/action.yml for all the available inputs.

## Examples

#### Typical Use Case

```yaml
- name: Checkout 
  uses: actions/checkout@v4
- uses: support-infinit/infinit-github-action@v1
  with:
    image: infinitsupport/infinit:latest
    options: -v ${{ github.workspace }}:/usr/src/app/www
    run: |
      node cli.js
```
