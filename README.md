Git Branch Assertion
===

A [Buildkite plugin](https://buildkite.com/docs/plugins) to check that the commit is "on the branch".
More specifically it checks that the commit is an ancestor of what the branch was pointing to at the time of checkout.

# Usage

Use the plugin in pipline upload step like this:

```yaml
steps:
  - command: buildkite-agent pipeline upload
    label: ':pipeline:'
    plugins:
      - triarius/branch-assertion: {}
```
