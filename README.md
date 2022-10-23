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

Overview of the entire flow:
<img width="1362" alt="Screenshot 2022-10-23 at 18 34 57" src="https://user-images.githubusercontent.com/1189998/197404226-11e41af7-25ad-4a96-82ae-ef740e735d4f.png">

How it looks to trigger a workflow manually, from https://github.com/famly/public-playground/actions/workflows/deployment-test.yml:
<img width="1179" alt="Screenshot 2022-10-23 at 18 31 29" src="https://user-images.githubusercontent.com/1189998/197404070-bcb3c4fb-e2a6-4e34-89b2-5902e52d284f.png">

How it looks to approve or reject a deployment review:
<img width="614" alt="Screenshot 2022-10-23 at 18 40 28" src="https://user-images.githubusercontent.com/1189998/197404454-1b2d3dd3-49ef-4a40-8a72-a34ba4ac9342.png">
