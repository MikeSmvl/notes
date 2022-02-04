# Usage

## [init](https://www.terraform.io/cli/commands/init)

```
terraform init
```

It’s  the  first  command  you  need  to  execute.  Otherwise,  terraform plan,  apply,  destroy  and  import  will  not  work. It is safe to run this command multiple times. &#x20;

The  command will  :

* find terraform  modules based on source provided
* configure and validate  a  backend (if present)
* install provider(s)  plugins

## [validate](https://www.terraform.io/cli/commands/validate)

```
terraform validate
```

Once you’ve initialized the directory, it’s a good idea to run the`validate` command before you run `plan` or `apply`. Validation catches syntax errors, version errors and more.

> It is safe to run this command automatically, for example as a post-save check in a text editor or as a test step for a re-usable module in a CI system.&#x20;

## [get](https://www.terraform.io/cli/commands/get)

This  command  is  useful  when you have  some  modules defined.

```
 terraform get ­
```

The modules are downloaded into a `.terraform` subdirectory of the current working directory. **Don't commit this directory to your version control repository.**

> `update=true` - If specified, modules that are already downloaded will be checked for updates and the updates will be downloaded if present.

## [plan](https://www.terraform.io/cli/commands/plan)

The  plan  command creates an execution plan which allows previewing changes. Like a dry run, it won't actually apply any of the proposed changes.

```
 terraform  plan ­
```

> By default, when Terraform creates a plan it:
>
> * Reads the current state of any already-existing remote objects to make sure that the Terraform state is up-to-date.
> * Compares the current configuration to the prior state and noting any differences.
> * Proposes a set of change actions that should, if applied, make the remote objects match the configuration.

## apply

Next comes the apply command which will execute the actions proposed in the plan.&#x20;

```
terraform apply
```

> `-auto-approve` - Skips interactive approval of plan before applying. This option is ignored when you pass a previously-saved plan file, because Terraform considers you passing the plan file as the approval and so will never prompt in that case.

Apply only one resource

```
terraform  apply -target="module.s3"
```

## Destroy

```
 terraform  destroy
```

This command deletes all the resources in the configuration.&#x20;

A  deletion  plan  can  be  created  before execution:

```
 terraform  plan  –destroy
```

Deletions can take a target resource too.

```
terraform  destroy - ­target=" aws_s3_bucket.my_bucket"
```
