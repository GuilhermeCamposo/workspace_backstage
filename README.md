# workspace_backstage
CHE workspace to be used for Backstage development


## how to access Backstage locally

    POD_NAME=$(oc get pod -l 'controller.devfile.io/devworkspace_name=backstage-dev' -o jsonpath='{.items[0].metadata.name}')
    oc port-forward pods/$POD_NAME 3000 7007


Backstage docs: https://backstage.io/docs/getting-started/ 

## [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn start
```