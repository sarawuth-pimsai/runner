# Github actions test runner

Download

```
# Create a folder
$ mkdir actions-runner && cd actions-runner# Download the latest runner package
$ curl -o actions-runner-osx-x64-2.288.1.tar.gz -L https://github.com/actions/runner/releases/download/v2.288.1/actions-runner-osx-x64-2.288.1.tar.gz# Optional: Validate the hash
$ echo "xxxxxxxxxxxxxxxxxx  actions-runner-osx-x64-2.288.1.tar.gz" | shasum -a 256 -c# Extract the installer
$ tar xzf ./actions-runner-osx-x64-2.288.1.tar.gz
```

Configure

```
# Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/sarawuth-pimsai/runner --token **************************# Last step, run it!
$ ./run.sh
```

Using your self-hosted runner
```
# Use this YAML in your workflow file for each job
runs-on: self-hosted
```