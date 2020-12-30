# ⚠️ Public ⚠️
Testing out GitHub features that require a public repository.

The `.github/workflows/environment-test.yml` workflow experiements with a deployment pipeline that branches between requiring a manual confirmation or being fully automatic, depending on the output of the first job in the workflow.

Check out the flow charts in the following cases:
- [A deployment that required a manual confirmation](https://github.com/famly/public-playground/actions/runs/452470323)
- [Output of first job was invalid](https://github.com/famly/public-playground/actions/runs/452467071) (makes sure we don't think a deployment has run when none has been triggered)
