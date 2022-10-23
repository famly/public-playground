# ⚠️ Public ⚠️
Testing out GitHub features that require a public repository.

The `.github/workflows/environment-test.yml` workflow experiements with a deployment pipeline that branches between requiring a [manual confirmation](https://docs.github.com/en/free-pro-team@latest/actions/managing-workflow-runs/reviewing-deployments) or being fully automatic, depending on the output of the first job in the workflow. With regards to manual approvals, CircleCI also has [something similar](https://circleci.com/docs/2.0/workflows/#holding-a-workflow-for-a-manual-approval) it seems.

Check out the flow charts in the following cases:

[A deployment that required a manual confirmation](https://github.com/famly/public-playground/actions/runs/452470323)
![A deployment that required a manual confirmation](https://user-images.githubusercontent.com/1189998/103345420-a0989680-4a91-11eb-90ae-3ad075407aa6.png)

[A deployment that was fully automated](https://github.com/famly/public-playground/actions/runs/452472723)
![A deployment that was fully automated](https://user-images.githubusercontent.com/1189998/103345416-a0000000-4a91-11eb-9a7a-3364cdb1d194.png)

[Output of first job was invalid](https://github.com/famly/public-playground/actions/runs/452467071) (makes sure we don't think a deployment has run when none has been triggered)
![Output of first job was invalid](https://user-images.githubusercontent.com/1189998/103345421-a1312d00-4a91-11eb-90f2-0fa94fba46ed.png)

# Continuous Deployment Flow

<img width="1363" alt="Screenshot 2022-10-23 at 18 04 11" src="https://user-images.githubusercontent.com/1189998/197402815-116c801b-249f-44be-85be-36e5183c827d.png">
