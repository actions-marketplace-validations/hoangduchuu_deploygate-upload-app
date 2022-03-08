<p align="center">
  <a href="https://github.com/jmatsu/dg-upload-app-action/actions"><img alt="typescript-action status" src="https://github.com/jmatsu/dg-upload-app-action/workflows/build-test/badge.svg"></a>
</p>

# Upload an app to DeployGate

This action uploads an application file to DeployGate.

## Inputs and Outpus

See *action.yml* of your version.

## Example

Please make sure your workflow will run when a branch is pushed.

```
on:
  push or pull_request
```

Add this action to steps.

```
- name: Upload Deploygate
        uses: minhchienwikipedia/deploygate-upload-app@master
        with:
          app_owner_name: postpay
          api_token: ${{ secrets.DEPLOYGATE_API_TOKEN }}
          app_file_path: file.ipa
          message: "Your note right here will show up on Deploygate"
```
