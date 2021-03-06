## kops create

Create a resource by filename or stdin.

### Synopsis


Create a resource by filename or stdin.

```
kops create -f FILENAME
```

### Examples

```
  # Create a cluster using a file
  kops create -f my-cluster.yaml
  
  # Create a cluster in AWS
  kops create cluster --name=example.com \
  --state=s3://kops-state-1234 --zones=eu-west-1a \
  --node-count=2 --node-size=t2.micro --master-size=t2.micro \
  --dns-zone=example.com
```

### Options

```
  -f, --filename stringSlice   Filename to use to create the resource
```

### Options inherited from parent commands

```
      --alsologtostderr                  log to standard error as well as files
      --config string                    config file (default is $HOME/.kops.yaml)
      --log_backtrace_at traceLocation   when logging hits line file:N, emit a stack trace (default :0)
      --log_dir string                   If non-empty, write log files in this directory
      --logtostderr                      log to standard error instead of files (default false)
      --name string                      Name of cluster
      --state string                     Location of state storage
      --stderrthreshold severity         logs at or above this threshold go to stderr (default 2)
  -v, --v Level                          log level for V logs
      --vmodule moduleSpec               comma-separated list of pattern=N settings for file-filtered logging
```

### SEE ALSO
* [kops](kops.md)	 - kops is kubernetes ops
* [kops create cluster](kops_create_cluster.md)	 - Create cluster
* [kops create instancegroup](kops_create_instancegroup.md)	 - Create instancegroup
* [kops create secret](kops_create_secret.md)	 - Create secrets

